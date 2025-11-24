# Ex01 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
models.py
---
from django.db import models
from django.contrib import admin 
class car(models.Model):
    regno=models.CharField(max_length=20,help_text="Car_ID")
    Car_Name=models.CharField(max_length=100)
    Price=models.IntegerField()
    year=models.IntegerField()
class CarAdmin(admin.ModelAdmin):
    list_display=('regno','Car_Name','Price','year')

admin.py
 ---   
from django.contrib import admin
from . models import car,CarAdmin
admin.site.register(car,CarAdmin)

# Register your models here.




## OUTPUT

[text](README.md) ![text](<Screenshot (54).png>)


## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
