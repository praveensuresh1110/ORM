# Ex02 Django ORM Web Application
## Date:18/12/2025
## ref no:25009816

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
~~~
models.py
from django.db import models
from django.contrib import admin
class Car (models.Model):
    model=models.CharField(max_length=20,primary_key="model")
    brand=models.CharField(max_length=100)
    price=models.IntegerField()
    year=models.IntegerField()
class CarAdmin(admin.ModelAdmin):
    list_display=('model','brand','price','year')
admin.py

from django.contrib import admin
from.models import Car,CarAdmin
admin.site.register(Car,CarAdmin) 
~~~


## OUTPUT
<img width="1920" height="1080" alt="Screenshot (60)" src="https://github.com/user-attachments/assets/357937be-09b4-4493-bb06-0f968814adfa" />




## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
