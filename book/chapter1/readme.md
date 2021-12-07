Table of Contents

```
1.1 The Importance of Making Your Code Readable . . . . . . . . . .  . . 1
1.2 PEP 8 . . . . . . . . . . . . . . . . . . . . . . . . .  . . . . . . 2
1.2.1 The 79-Character Limit . . . . . . . . . . . . . . . . . . . . . . 3
1.3 The Word on Imports . . . . . . . . . . . . . . . . . . . . .. . . . 4
1.4 Understand Explicit Relative Imports . . . . . . . . . . . . . . . . 5
1.5 Avoid Using Import * . . . . . . . . . . . . . . . . . . . . . . . . 6
1.5.1 Other Python Naming Collisions . . . . . . . . . . . . . . . . . . 7
1.6 Django Coding Style . . . . . . . . . . . . . . . . . . . . .. . . . 7
1.6.1 Consider the Django Coding Style Guidelines . . . . . . . . . . .. 8
1.6.2 Use Underscores in URL Pattern Names Rather Than Dashes . . . . .. 8
1.6.3 Use Underscores in Template Block Names Rather Than Dashes . . . . 9
1.7 Choose JS, HTML, and CSS Style Guides . . . . . . . . . . . . . . . .9
1.7.1 JavaScript Style Guides . . . . . . . . . . . . . . . . . . . . . .9
1.7.2 HTML and CSS Style Guides . . . . . . . . . . . . . . . . . . . . 10
1.8 Never Code to the IDE (Or Text Editor) . . . . . . . . . . . . . .. 10
1.9 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 10
```

### Habit of making 'readable'
- Avoid abbreviating variable names.
- Write out your function argument names.
- Document your classes and methods.
- Comment your code.
- Refactor repeated lines of code into reusable functions or methods.
- Keep functions and methods short. A good rule of thumb is that scrolling should not
be necessary to read an entire function or method.

* PEP 8
- “Use 4 spaces per indentation level.”
- “Separate top-level function and class definitions with two blank lines.”
- “Method definitions inside a class are separated by a single blank line.”

* 79-character limit

* Imports
1 Standard library imports
2 Related third-party imports
3 Local application or library-specific 

```python
# Stdlib imports
from math import sqrt
from os.path import abspath
# Core Django imports
from django.db import models
from django.utils.translation import gettext_lazy as _
# Third-party app imports
from django_extensions.db.models import TimeStampedModel
# Imports from your apps
from splits.models import BananaSplit
```

1 Standard library imports.
2 Imports from core Django.
3 Imports from third-party apps including those unrelated to Django.
4 Imports from the apps that you created as part of your Django project.

* absolute and explicit relative

```python
# cones/views.py
from django.views.generic import CreateView
# Relative imports of the 'cones' package
from .models import WaffleCone
from .forms import WaffleConeForm
# absolute import from the 'core' package
from core.views import FoodMixin
class WaffleConeCreateView(FoodMixin, CreateView):
model = WaffleCone
form_class = WaffleConeForm
```
Absolute imports are imports that point to a full path for a class or function.
Meaning they include every detail such as the folder(s) the module can be found 
in.
Absolute imports start from the parent directory of the project or the top level 
directory.
So suppose we have a directory structure such as 
```diff
└── project
    ├── package1
    │   ├── module1.py
    │   └── module2.py
    └── package2
        ├── __init__.py
        ├── module3.py
        ├── module4.py
        └── subpackage1
            └── module5.py
```
Using absolute imports, python starts searching for the module from the folder called
`project`.
Absolute imports begin with the folder name from which the module is located.
A Python module is a file that has a .py extension
Suppose we want to import a function called function1 which is located in the module3.py file
inside the package2 folder, then using absolute imports, we can import it using
```from package2.module3 import function1```
Python starts searching by opening the package2 folder and then locating the module3 file and 
then importing the function  `function1` from it.
Absolute imports are similar to normal paths on pc except the the slashes are replaced with 
periods(.)
Lets say a  path is represented on a windows pc as 
```bash
Desktop\DEV\projects\laboratorymanagement
```
In python, it will be translated to something such as `Desktop.DEV.projects.laboratorymanagement`
*One advantage of absolute imports is that they do not break the program even if the directory
structure is changed. For this reason it is recommended by PEP8*

Explicit Relative Imports.
Relative imports are relative to their current position, meaning they are relative to the file from
which you are using the import statement.
Unlike absolute imports that specify the name of the directory were modules are found, explicit relative
imports use the dot(.) notation to specify a location.
*A single dot meaning from the current directory.
Double dots(..) means from the directory before the the current directory and so on*

The advantage of explicit relative imports is that they are concise. 
But when the directory structure is changed, the program breaks since the item can no longer be found.
To show how explicit relative imports are concise, lets consider the same directory stucture.
```diff
└── project
    ├── package1
    │   ├── module1.py
    │   └── module2.py
    └── package2
        ├── __init__.py
        ├── module3.py
        ├── module4.py
        └── subpackage1
            └── module5.py
```
Suppose we were working in the package1 directory and wanted to import a function called funtion12 from the module module1, using relative imports 
we do something like
```python
from package1.module1 import function12
```
Using explicit relative imports, we would import it using 
```python
from .module1 import function12
```

```diff
@ You can see that using explicit relative imports, the line length has reduced.
+ In my opinion, explicit relative imports should only be used when impoting from modules in the current django application.
- To import modules from other apps, absolute imports should be used in order not to break the program when the file structure changes
```
```
