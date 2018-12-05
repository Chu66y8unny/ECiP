# C2

## Install and Run Python

Interactive Python <ipython.org>

```shell
$ # If using Conda package manager we should already have IPython
$ conda update ipython # update to the most recent version
$ # If Python is installed
$ pip install ipython
$ # If using Ubuntu
$ sudo apt-get install ipython 
```

```shell
$ ipython
$ python3
```

*What Every Computer Scientist Should Know About Floating-Point Arithmetic*, 
by David Goldberg.

## Special Variables

Four singletons: `True`, `False`, `None`, `NotImplemented`.

## Operators

```Python
del x
assert x
x.y
del x.y
x[y]
del x[y]
x in y
x not in y
x is y
x is not y
x < y < z
x if y else z
```

A string in Python 3 is an array of bytes and an associated encoding.

```Python
>>> help(slice)
```

## String

### String Literals
 
Any two string literals that are next to each other are stuck together automatically:
```Python
>>> "H + H"    " -> H2"
'H + H -> H2'
```

Newlines are ignored between parentheses. Long strings can be built up over multiple lines:
```Python
quote = ("Science is what we understand well enough to explain to a computer. "
         "Art is everything else we do. "
         "-Donald Knuth")
```

String literals can also be prefixed with `r`, `b`, `u`.

### String Methods

```Python
>>> help(str.strip)
>>> help(str.upper)
>>> help(str.lower)
>>> help(str.swapcase)
>>> help(str.isdigit)
>>> help(str.format)
```

## Modules

When a `.py` file is brought into a running Python interpreter, it is called 
a *module*. This is the in-memory representation of all of the Python code 
in the file. A collection of modules in a directory is called a *package*.

```Python
import <module>
<module>.foo
<module>.bar

from <module> import <var>
from <module> import <var1>, <var2>, ...
# use <var>, <var1>, <var2>
# equivalent to
import <module>
var = <module>.<var>
del <module>

import <module> as <name>
# equivalent to
import <module>
<name> = <module>
del <module>
<name>.foo
<name>.bar

from <module> import <var> as <name>
from <module> import <var1> as <name1>, <var2> as <name2>, ...
# equivalent to
from <module> import <var>
<name> = <var>
del <var>
```

## Packages

A collection of modules in the same directory is called a *package*. For the 
package to be visible to Python, the directory must contain a special file 
named `__init__.py`. The main purpose of the file is to signal to Python that 
the directory is a package, and that other files in this directory whose names 
end in `.py` are importable. This file does not need to have any code in it. 
If it does, this code will be executed before any other modules in the package 
are imported.

*absolute imports*

*implicit relative imports*

*explicit relative imports* the `from` keyword must be used, and the module 
name is prefixed by either `.` or `..`. `.` refers to the current package 
level. `..` refers to the package level one higher.

Useful modules in the Python standard library: `os`, `sys`, `math`, `re`, `subprocess`, `argparse`, `itertools`, `collections`, `decimal`, `random`, `csv`, `pdb`, `logging`


# C3


