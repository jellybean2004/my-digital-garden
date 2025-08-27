---
{"dg-publish":true,"permalink":"/content/013/e-gui/e2-signals-slots-and-events/","noteIcon":"1","created":"2025-08-27T13:15:28.438+01:00","updated":"2025-08-27T09:37:09.000+01:00"}
---

## signals and slots

>[!info] signals
>- notifications sent out by widgets when *something* happens

- this can be due to pressing a button, changing input text, etc.
- it can also send data for additional context
- custom signals can be made too

>[!info] slots
>- they are the receivers of signals

- any function/method can be used as a slot
- many Qt functions have built-in slots

```python
import sys
from PyQt6.QtWidgets import QApplication, QMainWindow, QPushButton

class MainWindow(QMainWindow):

    def __init__(self):
        super().__init__()
        
        self.button_is_checked = True ## to store the button status

        self.setWindowTitle("My App")
        
        button = QPushButton("Press Me!")
        button.setCheckable(True)
        button.clicked.connect(self.the_button_was_clicked)
        button.setChecked(self.button_is_checked)
        
        self.setCentralWidget(button)

    def the_button_was_clicked(self):
	    self.button_is_checked = True
    
        print("Clicked!")


app = QApplication(sys.argv)

window = MainWindow()
window.show()

app.exec()
```

- here, upon clicking the button (signal), `the_button_was_clicked` method (slot) is called
### changing the interface

```python
class MainWindow(QMainWindow):

    def __init__(self):
        super().__init__()

        self.setWindowTitle("My App")

        self.button = QPushButton("Press Me!")
        self.button.clicked.connect(self.the_button_was_clicked)
        
        self.setCentralWidget(self.button)
           

    def the_button_was_clicked(self):
        self.button.setText("You already clicked me.")
        self.button.setEnabled(False)

        self.setWindowTitle("New App")
```

- here, clicking the button changes the window title and the button text, and makes it unclickable

### connecting widgets together directly
- Qt widgets can be directly connected to another

```python
from PyQt6.QtWidgets import QApplication, QMainWindow, QLabel, QLineEdit, QVBoxLayout, QWidget

import sys


class MainWindow(QMainWindow):
    def __init__(self):
        super().__init__()

        self.setWindowTitle('my app')

        self.label = QLabel()

        self.input = QLineEdit()
        self.input.textChanged.connect(self.label.setText)

        layout = QVBoxLayout()
        layout.addWidget(self.input)
        layout.addWidget(self.label)
        
        container = QWidget()
        container.setLayout(layout)

        self.setCentralWidget(container)


app = QApplication(sys.argv)

window = MainWindow()
window.show()


app.exec()
```

- here, the `label` is directly connected to input

## events

>[!info] events
>- any interaction the user has with a Qt application

- these events are represented using **event objects** that package up information about what happened
- these are then passed to specific **event handlers**

- the event handlers for mouse events:

| event handler           | event type moved      |
| ----------------------- | --------------------- |
| `mouseMoveEvent`        | mouse moved           |
| `mousePressEvent`       | mouse button pressed  |
| `mouseReleaseEvent`     | mouse button released |
| `mouseDoubleClickEvent` | double click detected |
- these are only registered when a mouse button is pressed
- `setMouseTracking(True)` changes this behaviour
- all mouse events are tracked with the `QMouseEvent` object
