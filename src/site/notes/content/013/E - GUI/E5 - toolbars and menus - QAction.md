---
{"dg-publish":true,"permalink":"/content/013/e-gui/e5-toolbars-and-menus-q-action/","noteIcon":"1","created":"2025-08-27T13:15:28.453+01:00","updated":"2025-08-27T11:54:50.000+01:00"}
---

## toolbars
- `QAction` class allows defining abstract user interfaces
- this is better than using `QButton` as one only needs to define the triggered action once
- this can then be added to both the menu and the toolbar

```python
from PyQt6.QtCore import QSize, Qt
from PyQt6.QtGui import QAction, QIcon, QKeySequence
from PyQt6.QtWidgets import ( QApplication, QCheckBox, QLabel, QMainWindow, QStatusBar, QToolBar)


class Main(QMainWindow):

    def __init__(self):
        super().__init__()
        self.setWindowTitle("My App")

        toolbar = QToolBar("My Toolbar")
        self.addToolBar(toolbar)

        button_action = QAction("your button", self)
        button_action.setStatusTip('this is your button')
        button_action.triggered.connect(self.toolbar_button_clicked)
        button_action.setCheckable(True)
        toolbar.addAction(button_action)

        self.setStatusBar(QStatusBar(self)) ## shows status tip when hovering over the button

    
    def toolbar_button_clicked(self, s):
        print("clicked", s)
        
        
app = QApplication([])
window = Main()
window.show()
app.exec()
```

- icons can be added by passing the filename to the class, ie. `QIcon(filename)"`, and then passing it as the first argument, ie. `QAction(QIcon(filename), displayname,  self)`
## menubars
- now to add a menu bar item, the action can be reused

```python
	menu = self.menuBar()
	file_menu = menu.addMenu("&File")
	file_menu.addAction(button_action)
```

 - here, `alt + F` would jump to the menu item
 
>[!tip] accelerator keys
>adding `&` before a menu title enables user to jump to the menu item by pressing `alt`+ key

- `setKeySequence` can be used to add keyboard shortcuts for `QAction` 

```python
button_action.setShortcut(QKeySequence("Ctrl+p"))
```
