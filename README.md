# Ex02 Django ORM Web Application
## Date: 28-09-2024

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![image](https://github.com/user-attachments/assets/29aac959-5d6c-4d60-b05f-85acddb88a3b)



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
admin.py
```
from django.contrib import admin

from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)
```
models.py
```
from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.IntegerField(primary_key=True)
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
 
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')
```

## OUTPUT
![WhatsApp Image 2024-09-27 at 22 43 38_f0773b03](https://github.com/user-attachments/assets/a17e605e-3ff5-47ab-ab6f-4af4ef934ac7)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
