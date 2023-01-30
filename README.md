# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).


## Entity Relationship Diagram

![orm tree](https://user-images.githubusercontent.com/119407159/215472727-675affe0-bcfd-48dc-b3a1-07b7581cfb59.png)

## DESIGN STEPS
Step 1: create and collect customers infomartion using django application

Step 2: Implement that as Python code

Step 3: push that python code to github

PROGRAM

from django.db import models

# Create your models here. 
from django.db import models
from django.contrib import admin
# Create your models here.
class Customer(models.Model):
    customerid = models.CharField(max_length=8,primary_key=True)
    customername =models.CharField(max_length=100)
    mobilenumber =models.CharField(max_length=100)
    email = models.EmailField()
    quantity= models.IntegerField()
    

class CustomerAdmin(admin.ModelAdmin):
    list_display = ('customerid','customername','mobilenumber','email','quantity')

## OUTPUT

![orm custo](https://user-images.githubusercontent.com/119407159/215472793-3254545c-bb1d-4362-9dbf-4f822a41d6a9.png)

![orm cu](https://user-images.githubusercontent.com/119407159/215472824-3f34f6d5-e218-4615-a3ce-18a365ac0b73.png)

## RESULT
