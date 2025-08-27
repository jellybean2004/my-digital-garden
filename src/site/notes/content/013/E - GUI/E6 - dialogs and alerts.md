---
{"dg-publish":true,"permalink":"/content/013/e-gui/e6-dialogs-and-alerts/","noteIcon":"1","created":"2025-08-27T13:15:28.457+01:00","updated":"2025-08-27T12:16:42.000+01:00"}
---

>[!info] dialogs
>GUI components that allow one to communicate with the user

- handled by the `QDialog` class

```python
import sys

from PyQt6.QtWidgets import QApplication, QMainWindow, QPushButton, QDialog, QVBoxLayout


class MainWindow(QMainWindow):
    def __init__(self):
        super().__init__()

        self.setWindowTitle("My App")
        self.setFixedSize(400, 300)

        button = QPushButton("Open dialog!")
        button.clicked.connect(self.button_clicked)
        self.setCentralWidget(button)

    def button_clicked(self, s):
        print("click", s)

        dialog = QDialog()
        dialog.setWindowTitle("Hello!")
        dialog.setFixedSize(200, 100)
        dialog.exec()


app = QApplication(sys.argv)
window = MainWindow()
window.show()
app.exec()
```

>[!note]
>using `.exec()` to start the dialog starts a new event loop, which blocks the application execution

```python
class CustomDialog(QDialog):
    def __init__(self):
        super().__init__()

        self.setWindowTitle("Custom Dialog")
        self.setFixedSize(200, 100)

        QBtn = (
            QDialogButtonBox.StandardButton.Ok | 
            QDialogButtonBox.StandardButton.Cancel
        )

        self.buttonBox = QDialogButtonBox(QBtn)
        self.buttonBox.accepted.connect(self.accept)
        self.buttonBox.rejected.connect(self.reject)

        layout = QVBoxLayout()
        message = QLabel("Something happened, is that OK?")
        layout.addWidget(message)
        layout.addWidget(self.buttonBox)
        self.setLayout(layout)


class MainWindow(QMainWindow):

    # ... add the following method after the __init__

    def button_clicked(self, s):
        print("click", s)

        dlg = CustomDialog()
        if dlg.exec():
            print("Success!")
        else:
            print("Cancel!")
```