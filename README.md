# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
clone the experiment from github
### STEP 2:
enter code in models.py and admins.py
### STEP 3:

Write your own steps

## PROGRAM
```html
<!DOCTYPE html>
<html>
    <head></head>
    <body>
        <h1>
            Welcome to Saveetha Engineering College
        </h1>
    </body>
</html>


```
### models
```python
from django.db import models
from django.contrib import admin

# Create your models here.
class Student (models.Model):
    referencenumber=models.CharField(max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()


class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email')
```
### admins
```python
from django.contrib import admin
from .models import Student,StudentAdmin

# Register your models here.
admin.site.register(Student,StudentAdmin)
```
## OUTPUT

### serveroutput
![](./so.png)
### clientoutput
![](./co.png)


## RESULT
