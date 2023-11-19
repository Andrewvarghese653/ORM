# Ex02 Django ORM Web Application
## Date: 
14.09.2023

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## Entity Relationship Diagram


## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM
```

from django.db import models
from django.contrib import admin
class employement(models.Model):
    employementnumber = models.IntegerField(max_length=10)
    employementname = models.CharField(max_length=100)
    age = models.IntegerField() 
    email = models.EmailField()
    place = models.CharField(max_length=100)
    designation = models.CharField(max_length=100)
    salary = models.CharField(max_length=100)
class EmployementAdmin(admin.ModelAdmin):
    list_display = ('employementnumber','employementname','age','email','place','designation','salary')
```
code in admin.py
```
from django.contrib import admin
from .models import employement,EmployementAdmin
admin.site.register(employement,EmployementAdmin)


```

## OUTPUT

<img width="829" alt="Screenshot 2023-11-19 at 10 14 44 PM" src="https://github.com/Andrewvarghese653/ORM/assets/145822115/1fe53679-cec6-4750-89cb-30df2e1d0546">



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
