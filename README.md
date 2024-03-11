EX02 # Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![WhatsApp Image 2024-03-11 at 21 55 12_ebe58e37](https://github.com/HARISHA2006/harisha/assets/148843830/637994f7-014b-4def-9fb6-29cda7f1bf04)



## DESIGN STEPS

### STEP 1:
Clone the problem from github

### STEP 2:
create a new app

### STEP 3:
Enter the code for admin.py and model.py

### STEP 4:
Execute Django admin and create 10 employees

## PROGRAM

```
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
```

admin.py

from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

```

## OUTPUT
![Screenshot 2024-03-11 203829](https://github.com/HARISHA2006/harisha/assets/148843830/0d01c72d-3cbe-4574-955e-3c58c2e41c8c)

## RESULT

Thus the program for creating a database using ORM hass been executed successfully
