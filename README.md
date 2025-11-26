# Ex02 Django ORM Web Application
# Date:
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 cars

# PROGRAM
```
models.py
from django.db import models
from django.contrib import admin
class car (models.Model):
    owner = models.CharField(max_length=100)
    make = models.CharField(max_length=100)
    model = models.CharField(max_length=100)
    year = models.IntegerField()

class carAdmin (admin.ModelAdmin):
    list_display = ('owner', 'make', 'model', 'year')


admin.py
from django.contrib import admin
from .models import car,carAdmin
admin.site.register(car, carAdmin)
```
# OUTPUT
![WhatsApp Image 2025-11-26 at 20 48 36_cfc04df1](https://github.com/user-attachments/assets/859c3dbf-7303-4e2a-bb83-b527eaf5bfe7)
![WhatsApp Image 2025-11-26 at 20 48 36_ba1b40fa](https://github.com/user-attachments/assets/baee1548-18f3-46d7-bcd0-9a8a73cfa3a6)



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
