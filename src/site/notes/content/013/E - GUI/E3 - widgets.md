---
{"dg-publish":true,"permalink":"/content/013/e-gui/e3-widgets/","noteIcon":"1","created":"2025-08-27T09:37:25.803+01:00","updated":"2025-08-27T09:50:06.474+01:00"}
---

>[!info] widget
>a UI component that a user can interact with

| widget           | what it does                            |
| ---------------- | --------------------------------------- |
| `QCheckbox`      | a checkbox                              |
| `QComboBox`      | a dropdown list box                     |
| `QDateEdit`      | for editing dates and datetimes         |
| `QDateTimeEdit`  | for editing dates and datetimes         |
| `QDial`          | rotatable dial                          |
| `QDoubleSpinBox` | a number spinner for floats             |
| `QFontComboBox`  | a list of fonts                         |
| `QLCDNumber`     | a quite ugly LCD display                |
| `QLabel`         | just a label, not interactive           |
| `QLineEdit`      | enter a line of text                    |
| `QProgressBar`   | a progress bar                          |
| `QPushButton`    | a button                                |
| `QRadioButton`   | a toggle set, with only one active item |
| `QSlider`        | a slider                                |
| `QSpinBox`       | an integer spinner                      |
| `QTimeEdit`      | for editing times                       |
*table: [python guis](https://www.pythonguis.com/tutorials/pyqt6-widgets)*

- alignments are specified by using a flag

| pyqt6 flag (long name)          | behavior                                     |
| ------------------------------- | -------------------------------------------- |
| `Qt.AlignmentFlag.AlignLeft`    | aligns with the left edge.                   |
| `Qt.AlignmentFlag.AlignRight`   | aligns with the right edge.                  |
| `Qt.AlignmentFlag.AlignHCenter` | centers horizontally in the available space. |
| `Qt.AlignmentFlag.AlignJustify` | justifies the text in the available space.   |
| `Qt.AlignmentFlag.AlignTop`     | aligns with the top.                         |
| `Qt.AlignmentFlag.AlignBottom`  | aligns with the bottom.                      |
| `Qt.AlignmentFlag.AlignVCenter` | centers vertically in the available space.   |
| `Qt.AlignmentFlag.AlignCenter`  | centers horizontally and verically           |

- pipes can be used to combine horizontal and vertical alignment flags

```python
align_top_right = Qt.AlignmentFlag.AlignLeft | Qt.AlignmentFlag.AlignTop
```

