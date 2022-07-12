# KCE-Multi-Study

Don't Read this, it is not related to you.😅🤷‍♂️
...Pehli fursat me nikal  ....

#############   PYTHON PRACTICALS
***********    Practical 1

Program Name: Write a Program to calculate area of circle, rectangle, triangle.

import math
print("\n Choose any one  \n\n\n")


print("1. Radius of circle \n")
print("2. Radius of Triangle \n")
print("3. Radius of Squere \n")

ch=int(input("Enter ur choice :  "))

if(ch==1):
    
     r=float(input("Enter radius of circle : "))
     sol=3.14*pow(r,2)
     # print(f"Area {r} is : {round(sol,3)}")     we can also write with this formate.

     print("Area of circle : ",round(sol,3))
    
if(ch==2):
    
     h,b=float(input("Enter Hight of Triangle : ")),float(input("Enter Base of Triangle : "))
     sol=.5*b*h
     print("Area of circle : ",round(sol,3))

if(ch==3):
    
     w,h=float(input("Enter width of Squere : ")),float(input("Enter hight of Squere : "))
     sol=w*h
     print("Area of circle : ",round(sol,3))


##############  PRACTICAL 2 ##############

