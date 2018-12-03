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
