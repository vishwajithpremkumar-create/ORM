# Ex02 Django ORM Web Application
## Date: 05-10-2025

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
from django.db import models
from django.contrib import admin

class Car(models.Model):
    car_brand = models.CharField()
    car_model = models.CharField()
    year = models.DateField
    color = models.CharField()
    engine_type = models.CharField()
    fuel_type = models.CharField()
    transmission = models.CharField()
    seating_capacity = models.IntegerField()
    price = models.CharField()
    mileage = models.CharField()
    description = models.CharField()

class CarAdmin(admin.ModelAdmin):
    list_display = ('car_brand', 'car_model', 'year', 'color','engine_type', 'fuel_type', 'transmission', 'price','mileage','description')

admin.py
from django.contrib import admin
from.models import(Car,CarAdmin)
admin.site.register(Car,CarAdmin)



## OUTPUT
![alt text](<Screenshot 2025-09-16 223204.png>)

Include the screenshot of your admin page.


## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
