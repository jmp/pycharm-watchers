# PyCharm File Watchers

This repository contains some [file watchers][1] for [PyCharm][2] I've found useful.

## Included watchers

* Format the current file using [black][3]
* Reorder imports in the current file using [isort][4]

## Requirements

To use these file watchers, the active Python environment (e.g. project-specific virtual environment)
should have `black` and `isort` installed. The file watchers will try to run the `black` and `isort`
binaries in the current interpreter directory (`$PyInterpreterDirectory$/black` and `$PyInterpreterDirectory$/isort`).

## Installation

1. Download the `watchers.xml` file
2. Open *Preferences* > *File Watchers* and click *Import*
3. Select `watchers.xml`
4. Click *Apply* to save the changes

The file watchers should execute the next time the a Python file is saved. For security purposes, PyCharm
will ask you to trust the file watchers the first time they are triggered.

[1]: https://jetbrains.com/help/pycharm/using-file-watchers.html
[2]: https://jetbrains.com/pycharm/
[3]: https://github.com/psf/black
[4]: https://github.com/PyCQA/isort
