# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![erdiagram](https://user-images.githubusercontent.com/119405626/215393568-aa094a05-94af-4bbe-ab3a-b80b7c7bc882.png)


## DESIGN STEPS

### STEP 1:
First go to student.saveetha.ac.in and open theiaIDE
### STEP 2:
Open theiaIDE and go to admin.py and open models.py put some comments
### STEP 3:

Open github.com and create and generate classic token

## PROGRAM
python
```
class Employee(models.Model):
    emp_id=models.CharField(primary_key=True,max_length=4,help_text="Employee ID")
    ename=models.CharField(max_length=50)
    post=models.CharField(max_length=20)
    salary=models.IntegerField()
    age=models.IntegerField()


class EmployeeAdmin(admin.ModelAdmin):
    list_display=('emp_id','ename','post','salary','age')
```
python
```
from django.db import models
from django.contrib import admin
# Register your models here.
admin.site.register(Employee,EmployeeAdmin)
```
## OUTPUT

![orm2](https://user-images.githubusercontent.com/119405626/215393397-7099eba7-d862-4c99-b0ac-510d19ccc9f4.png)


## RESULT
I developed a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).
