### Python skills

This is basic skills for Python programming language 

#### 1. Doctest
Doctest is a module included in the Python programming language's standard library that
allows the easy generation of tests based on output from the standard Python interpreter shell,
cut and pasted into [docstring](https://en.wikipedia.org/wiki/Docstring)

When using the Python shell:
+ the primary prompt: `>>>`, is followd by new commands
+ the secondary prompt: `...`, is used when continuing commands o multiple lines, the results of executing the command
is expected on following lines.
  
###### Example 1: A doctest embedded in the docstring of a function
```python
def func_compare_lambda(x):
    """
    The lambda keyword is used to create inline function
    
    
    'Lambda function ideal for use in callbacks, and when 
    functions are to bo passed as arguments to other functions'
    
    >>> def square_func(x):
    ...    return x * x
    >>> square_ld = lambda x: x * x
    >>> for i in range(10):
    ...    assert square_func(i) == square_ld(i)
    >>>
    """
```

###### Example 2: Doctests embedded in a README.txt file
```markdown
======================
Demonstration doctests
======================

This is just an example of what a README text looks like that can be used with
the doctest.DocFileSuite() function from Python's doctest module.

Normally, the README file would explain the API of the module, like this:

>>> a = 1
>>> b = 2
>>> a + b
3

Notice, that we just demonstrated how to add two numbers in Python, and 
what the result will look like.

A special option allows you to be somewhat fuzzy about your examples:

>>> o = object()
>>> o               
<object object at 0x...>

Exceptions can be tested very nicely too:

>>> x
Traceback (most recent call last):
 ...
NameError: name 'x' is not defined
```

#### 2. Build-in function `any()` and `all()` on a list



