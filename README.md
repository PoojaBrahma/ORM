# Ex02 Django ORM Web Application
# Date:19/10/2024
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
```python
models.py

from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,help_text="Employee_ID")
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_disply=('eid','name','salary','age','email')


admin.py

from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)
```
# OUTPUT
![Screenshot 2024-12-05 235409](https://github.com/user-attachments/assets/2b0a4938-41b9-40cd-a55c-88a8e19cef1a)
![Screenshot 2024-12-07 155014](https://github.com/user-attachments/assets/75e4d90a-a694-4008-a0b5-38fb3f6487ce)
![Screenshot 2024-12-07 155039](https://github.com/user-attachments/assets/4ce9a0fd-daeb-47e9-8da6-05a4bcadf1d1)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
