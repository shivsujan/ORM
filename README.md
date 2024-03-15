# Ex02 Django ORM Web Application
## Date: 29/02/2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![Uploading Screenshot 2024-03-15 123309.png…]()

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
```
admin.py

from django.contrib import admin
from .models import Book ,BookAdmin
admin.site.register(Book,BookAdmin)


models.py

from django.db import models
from django.contrib import admin
class Book(models.Model):
     bookid=models.IntegerField(primary_key=True);
     bookname=models.CharField(max_length=20);
     author=models.CharField(max_length=50);
     price=models.IntegerField();
     publishdate=models.DateField();
class BookAdmin(admin.ModelAdmin):
     list_display=("bookid","bookname","author","price","publishdate");

```

## OUTPUT
![web application 2](https://github.com/shivsujan/ORM/assets/145633245/f310108f-1d8e-45e4-b1b6-e2af116b208d)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
