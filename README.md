# lineditor
[![Python Versions](https://img.shields.io/pypi/pyversions/lineditor.svg)](https://pypi.org/project/lineditor/)
[![PyPI version](https://badge.fury.io/py/lineditor.svg)](https://badge.fury.io/py/lineditor)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Simple library to edit or read text of specific line.

2020/12/20 - Now lineditor available on PyPI !

## Install
A. From PyPI ( stable )

`pip install lineditor`

B. From GitHub ( latest )

`git clone https://github.com/mafusuke/lineditor.git && cd lineditor && pip install -e .`

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