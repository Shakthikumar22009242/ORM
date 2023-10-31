# Ex02 Django ORM Web Application
## Date: 07.10.2023

## AIM
To develop a Django application to store and retrieve data from a 
Football Players database using Object Relational Mapping(ORM).

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
```python
Admin.py
from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

Models.py
from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,help_text="Employee ID")
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')
```



## OUTPUT

![WEB_EX02](https://github.com/Shakthikumar22009242/ORM/assets/120207509/918dcd35-a730-4798-88e6-2d0c88190c82)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
