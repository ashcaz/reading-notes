# Django Models

**LINKS**

- [Using Models](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models)
- [Django Admin](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Admin_site)

- [Beginner’s Guide to Django - Part 1](https://simpleisbetterthancomplex.com/series/2017/09/04/a-complete-beginners-guide-to-django-part-1.html)
- [Video: Beginner’s Guide to Django - Part 2](https://simpleisbetterthancomplex.com/series/2017/09/11/a-complete-beginners-guide-to-django-part-2.html)

## Using Models

### Model Definition

Models are usually defined in an application's models.py file. They are implemented as subclasses of `django.db.models.Model`, and can include fields, methods and metadata. The code fragment below shows a "typical" model, named `MyModelName`:

```Python
from django.db import models

class MyModelName(models.Model):
    """A typical class defining a model, derived from the Model class."""

    # Fields
    my_field_name = models.CharField(max_length=20, help_text='Enter field documentation')
    ...

    # Metadata
    class Meta:
        ordering = ['-my_field_name']

    # Methods
    def get_absolute_url(self):
        """Returns the url to access a particular instance of MyModelName."""
        return reverse('model-detail-view', args=[str(self.id)])

    def __str__(self):
        """String for representing the MyModelName object (in Admin site etc.)."""
        return self.my_field_name
```

**Common field arguments**

The following common arguments can be used when declaring many/most of the different field types:

- `help_text`: Provides a text label for HTML forms (e.g. in the admin site), as described above.
- `verbose_name`: A human-readable name for the field used in field labels. If not specified, Django will infer the default verbose name from the field name.
- `default`: The default value for the field. This can be a value or a callable object, in which case the object will be called every time a new record is created.
- `null`: If True, Django will store blank values as NULL in the database for fields where this is appropriate (a CharField will instead store an empty string). The default is False.
- `blank`: If True, the field is allowed to be blank in your forms. The default is False, which means that Django's form validation will force you to enter a value. This is often used with null=True , because if you're going to allow blank values, you also want the database to be able to represent them appropriately.
- `choices`: A group of choices for this field. If this is provided, the default corresponding form widget will be a select box with these choices instead of the standard text field.
- `primary_key`: If True, sets the current field as the primary key for the model (A primary key is a special database column designated to uniquely identify all the different table records). If no field is specified as the primary key then Django will automatically add a field for this purpose.

## Django Admin

### Registering models

First, open `admin.py` in the catalog application (**/locallibrary/catalog/admin.py**). It currently looks like this — note that it already imports `django.contrib.admin`:

```Python
from django.contrib import admin

# Register your models here.
```

Register the models by copying the following text into the bottom of the file. This code imports the models and then calls `admin.site.register` to register each of them.

```Python
from .models import Author, Genre, Book, BookInstance

admin.site.register(Book)
admin.site.register(Author)
admin.site.register(Genre)
admin.site.register(BookInstance)
```

This is the simplest way of registering a model, or models, with the site. The admin site is highly customisable, and we'll talk more about the other ways of registering your models further down.

[Back to Homepage](https://ashcaz.github.io/reading-notes)
