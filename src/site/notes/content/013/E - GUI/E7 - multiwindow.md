---
{"dg-publish":true,"permalink":"/content/013/e-gui/e7-multiwindow/","noteIcon":"1","created":"2025-08-27T13:25:06.302+01:00","updated":"2025-08-27T14:23:23.453+01:00"}
---

- any widget without a parent is a window

```python
from PyQt6.QtWidgets import QApplication, QMainWindow, QPushButton, QLabel, QVBoxLayout, QWidget

import sys

class AnotherWindow(QWidget):

    def __init__(self):
    
        super().__init__()
        self.setWindowTitle("Another Window")
        self.resize(400, 300)
        
        layout = QVBoxLayout()
        self.setLayout(layout)
        self.label = QLabel("This is another window")
        layout.addWidget(self.label)
        
        
class MainWindow(QMainWindow):

    def __init__(self):
        super().__init__()
        self.setWindowTitle("Main Window")
        self.resize(400, 300)
        
        self.button = QPushButton("Open Another Window")
        self.button.clicked.connect(self.open_another_window)
        self.setCentralWidget(self.button)
        
        
    def open_another_window(self):
        another_window = AnotherWindow()
        another_window.show()
        
        
app = QApplication(sys.argv)
window = MainWindow()
window.show()
app.exec()
```

- here, the window only opens for a fraction of a second
- this is due to it being a local variable that is wiped up

```python
    def open_another_window(self):
        self.another_window = AnotherWindow()
        self.another_window.show()
```

- this will make the new window persist
- but when the button is pressed again, it get closed as the new window replaces the current variable

```python
class MainWindow(QMainWindow):

    def __init__(self):
    
        super().__init__()
        self.setWindowTitle("Main Window")
        self.resize(400, 300)
        
        self.another_window = None
        
        self.button = QPushButton("Open Another Window")
        self.button.clicked.connect(self.open_another_window)
        self.setCentralWidget(self.button)
        
    def open_another_window(self):
    
        if self.another_window is None:
            self.another_window = AnotherWindow()
        self.another_window.show()
        
```

- now, a new window will only be opened if there is no other window open


```python

from random import randint


class AnotherWindow(QWidget):
    
    def __init__(self):
        
        super().__init__()
        self.setWindowTitle("Another Window")
        self.resize(400, 300)
        layout = QVBoxLayout()
        self.setLayout(layout)
        self.label = QLabel("This is another window % d" % randint(0, 100))
        layout.addWidget(self.label)
        
        
class MainWindow(QMainWindow):
    
    def __init__(self):
        
        super().__init__()
        self.setWindowTitle("Main Window")
        self.resize(400, 300)
        
        self.another_window = AnotherWindow()

        self.button = QPushButton("Open Another Window")
        self.button.clicked.connect(self.toggle_window)
        self.setCentralWidget(self.button)
        
            
    def toggle_window(self):
            
            if self.another_window.isVisible():
                self.another_window.hide()
            else:
                self.another_window.show()
```

- the above code creates a togglable window

```python
class MainWindow(QMainWindow):
    
    def __init__(self):
        
        super().__init__()
        self.setWindowTitle("Main Window")
        self.resize(400, 300)
        
        self.another_window1 = AnotherWindow()
        self.another_window2 = AnotherWindow()
        
        layout = QVBoxLayout()
        
        self.button1 = QPushButton("Open Another Window 1")
        self.button1.clicked.connect(self.toggle_window1)
        
        self.button2 = QPushButton("Open Another Window 2")
        self.button2.clicked.connect(self.toggle_window2)
        
        layout.addWidget(self.button1)
        layout.addWidget(self.button2)
        
        w = QWidget()
        w.setLayout(layout)
        self.setCentralWidget(w)
        
            
    def toggle_window1(self):
            
            if self.another_window1.isVisible():
                self.another_window1.hide()
            else:
                self.another_window1.show()
                
    def toggle_window2(self):
            
            if self.another_window2.isVisible():
                self.another_window2.hide()
            else:
                self.another_window2.show()
```

- here, two buttons, each toggling a separate window, are added

