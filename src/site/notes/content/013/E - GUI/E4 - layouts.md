---
{"dg-publish":true,"permalink":"/content/013/e-gui/e4-layouts/","noteIcon":"1","created":"2025-08-27T13:15:28.448+01:00","updated":"2025-08-27T10:35:47.000+01:00"}
---

- the four basic layout types:

| layout          | behavior                          |
|-----------------|-----------------------------------|
| QHBoxLayout     | linear horizontal layout          |
| QVBoxLayout     | linear vertical layout            |
| QGridLayout     | in indexable grid xxy             |
| QStackedLayout  | stacked (z) in front of one another|

![grid layout.png|500](/img/user/pics/grid%20layout.png)
*image: [Python GUIs](https://www.pythonguis.com/tutorials/pyqt6-layouts/)*

```python
import sys

from PyQt.QtWidgets import QWidget

from PyQt6.QtGui import QColor, QPalette


class Color(QWidget):
    def __init__(self, color):
        super().__init__()
        self.setAutoFillBackground(True)

        palette = self.palette()
        palette.setColor(QPalette.ColorRole.Window, QColor(color))
        self.setPalette(palette)
        
        import sys
```

- this creates  a widget subclass that creates a solid-filled widget as follows: `Color('red`

```python
ffrom PyQt6.QtWidgets import QApplication, QMainWindow, QTabWidget


class MainWindow(QMainWindow):
    def __init__(self):
        super().__init__()

        self.setWindowTitle("My App")

        tabs = QTabWidget()
        tabs.setTabPosition(QTabWidget.TabPosition.West)
        tabs.setMovable(True)

        for color in ["red", "green", "blue", "yellow"]:
            tabs.addTab(Color(color), color)

        self.setCentralWidget(tabs)


app = QApplication(sys.argv)
window = MainWindow()
window.show()
app.exec()
```


- this creates a layout with tabs on the left that change the color of the widget when clicked

![E4 - layouts.png|250](/img/user/pics/E4%20-%20layouts.png)