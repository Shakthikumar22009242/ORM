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
Admin.py
```python
from django.contrib import admin
from .models import football,footballAdmin
admin.site.register(football,footballAdmin)
```

Models.py
```python
from django.db import models
from django.contrib import admin
class football (models.Model):
    name=models.CharField(max_length=20,help_text="Player ID")
    role=models.CharField(max_length=100)
    Jersey_no=models.IntegerField()
    goals=models.IntegerField()

class footballAdmin(admin.ModelAdmin):
    list_display=('Jersey_no','name','goals','role')

```


## OUTPUT
![Screenshot (262)](https://github.com/Shakthikumar22009242/ORM/assets/120207509/f949fff8-4ada-46d5-994b-9a5d02ee7aaf)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
