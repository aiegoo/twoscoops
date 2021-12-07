Table of Contents

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

### Habit of making 'readable'
- Avoid abbreviating variable names.
- Write out your function argument names.
- Document your classes and methods.
- Comment your code.
- Refactor repeated lines of code into reusable functions or methods.
- Keep functions and methods short. A good rule of thumb is that scrolling should not
be necessary to read an entire function or method.

* PET 8
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