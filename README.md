# Ex02 Django ORM Web Application
## Date: 20/9/2025

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).




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
from .models import Movies, MoviesAdmin
admin.site.register(Movies,MoviesAdmin)


models.py

from django.db import models
from django.contrib import admin
class Movies(models.Model):
    M_ID = models.IntegerField(primary_key=True)
    M_name = models.CharField(max_length=100)
    Release_date=models.DateField()
    Director=models. CharField(max_length=50)
    Actors=models. CharField(max_length=100)
 
class MoviesAdmin(admin.ModelAdmin):
    list_display=('M_ID','M_name','Release_date', 'Director','Actors')
```

## OUTPUT

<img width="1286" height="723" alt="Screenshot 2025-09-20 134224" src="https://github.com/user-attachments/assets/cfe693c1-a72b-4a97-8238-1f8560c7be36" />



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
