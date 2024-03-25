# Ex02 Django ORM Web Application
## Date: 28.2.24

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![WhatsApp Image 2024-03-25 at 15 07 58_32e39d7a](https://github.com/Mohanraj2006/ORM/assets/152195759/a000a8f1-35ab-4e03-ba7a-9c5274ea41d0)


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
from .models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)

models.py
from django.db import models
from django.contrib import admin
class Book_DB(models.Model):
     serialno=models.IntegerField(primary_key="serialno");
     bookname=models.CharField(max_length=20);
     publisher=models.CharField(max_length=20);
     Dop=models.DateField();
     totalpg=models.IntegerField();
class Book_DBAdmin(admin.ModelAdmin):
     list_display=("serialno","bookname","publisher","Dop","totalpg");
```

## OUTPUT
![alt text](<Screenshot (3).png>)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
