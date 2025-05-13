# Ex02 Django ORM Web Application
## Date: 24.04.2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).





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
from .models import Movie,MovieAdmin

admin.site.register(Movie,MovieAdmin)

models.py

from django.db import models
from django.contrib import admin

class Movie(models.Model):
    title=models.CharField(max_length=150,primary_key='True')
    genre=models.CharField(max_length=100)
    release_date=models.DateField()
    rating=models.IntegerField()
    
class MovieAdmin(admin.ModelAdmin):
    list_display=('title','genre','release_date','rating')



```

## OUTPUT

![image](https://github.com/user-attachments/assets/5a4f94f4-418e-4691-9bd8-1018ee22ddb3)


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
