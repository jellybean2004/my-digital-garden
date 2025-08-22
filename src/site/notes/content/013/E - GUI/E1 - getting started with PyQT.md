---
{"dg-publish":true,"permalink":"/content/013/e-gui/e1-getting-started-with-py-qt/","noteIcon":"1","created":"2025-08-22T11:03:36.805+01:00","updated":"2025-08-22T11:51:17.626+01:00"}
---

### event loop
- `QApplication` class is the core of every QT application
- only one instance is needed
- it holds the **event loop** - the core loop which governs the user interaction with the GUI

![event loop.png|500](/img/user/pics/event%20loop.png)
*image: [pythonguis](https://www.pythonguis.com/tutorials)*

- each interaction generates an **event**, placed on the **event queue**
- the event handler deals with the event, and passes the control back to the loop to wait for more events

```python
import sys
from PyQt6.QtWidgets import QApplication, QPushButton

## creating an instance of the application
app = QApplication(sys.argv)

## creating an instance of a button
window = QPushButton("Push Me")
window.show() #hidden by default

## start the event loop
app.exec()
```

- to create custom windows, subclass `QMainWindow`

```python
## creating a sub class
class MainWindow(QMainWindow):

	##including the setup, allwing the window behviour to be self contained
    def __init__(self):
        super().__init__()

        self.setWindowTitle("My App")
        
        button = QPushButton("Press Me!")
        
        self.setFixedSize(QSize(400, 300)) # set the window size to 400x300 px
        self.setMinimumSize(QSize(200, 300))
        self.setMaximumSize(QSize(600, 300))  

        ## set the central widget of the window.
        self.setCentralWidget(button)
        
        
## assigning the subclass to a variable
window = MainWindow()
window.show()
```