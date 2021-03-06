# lineditor
[![Python Versions](https://img.shields.io/pypi/pyversions/lineditor.svg)](https://pypi.org/project/lineditor/)
[![PyPI version](https://img.shields.io/pypi/v/lineditor)](https://pypi.org/project/lineditor/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Simple library to edit or read text of specific line.

2020/12/20 - Now lineditor available on PyPI !

## Install
A. From PyPI ( stable )

`pip install lineditor`

B. From GitHub ( latest )

`pip install git+https://github.com/mafusuke/lineditor.git`

## Sample Usage
```python
import lineditor

# load the target file
file = lineditor.Editor("./hoge.txt")

# print the string on the 10th line
print(file[10])
# modify the string on the 21th line into "new text"
file[21] = "new text"
# total lines count of the file
print(len(file)) 
```