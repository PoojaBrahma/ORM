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
``` python
models.py:

from django.db import models
from django.contrib import admin
class bankloan(models.Model):
    Name=models.CharField(max_length=100)
    Accountno=models.IntegerField(primary_key="Accountno")
    Startdate=models.DateField()
    Email=models.EmailField()
    Mobilenumber=models.IntegerField()
    Amount=models.IntegerField()

class bankloanAdmin(admin.ModelAdmin):
    list_display=('Name','Accountno','Startdate','Email','Mobilenumber','Amount')


admin.py:

from django.contrib import admin
from .models import bankloan,bankloanAdmin
admin.site.register(bankloan,bankloanAdmin)
```
# OUTPUT
![WhatsApp Image 2024-12-07 at 10 48 41 PM](https://github.com/user-attachments/assets/ce054704-566b-4995-8332-e009eb5b9213)

![Screenshot 2024-12-07 230142](https://github.com/user-attachments/assets/99e1f565-9785-45b1-a337-efc6ba2f5471)

![Screenshot 2024-12-07 233409](https://github.com/user-attachments/assets/44537609-64a9-4a71-9cb3-4cc766da5817)

![Screenshot 2024-12-05 235409](https://github.com/user-attachments/assets/72012fcf-f2a7-4142-b6f3-f6199ec5513c)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully.
