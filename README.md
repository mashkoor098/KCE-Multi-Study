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

# intersction of 2 list 

def intersection_list(list1, list2):  
   return list(set(list1) & set(list2))  
  
list1 = [40, 90, 11, 58, 31, 66, 28, 54, 79]  
list2 = [58, 90, 54, 31, 45, 11, 66, 28, 26]  
  
print(intersection_list(list1, list2))


##############  PRACTICAL 3 ##############

# Write Program to count the occurrences of each word in a given string sentence.

def word_count(str):
    counts = dict()
    words = str.split()

    for word in words:
        if word in counts:
            counts[word] += 1
        else:
            counts[word] = 1

    return counts

print( word_count('the quick brown fox jumps over the lazy dog.'))

##############  PRACTICAL 4 ##############

# find sub-string is present in string or not.

string=input("Enter string:")
sub_str=input("Enter word:")
if(string.find(sub_str)==-1):
      print("Substring not found in string!")
else:
      print("Substring in string!")
      
##############  PRACTICAL 5 ##############

#Union of 2 list

def Union(lst1, lst2):
    final_list = lst1 + lst2
    return final_list


lst1 = [23, 15, 2, 14, 14, 16, 20 ,52]
lst2 = [2, 48, 15, 12, 26, 32, 47, 54]
print("union of lst is:",Union(lst1, lst2))


##############  PRACTICAL 6 ##############

# Program Name: Write Program to remove all tuples in a list of tuples with the USN outside the given range.

y=[('a','12CS039'),('b','12CS320'),('c','12CS055'),('d','12CS100')]

low=int(input("Enter lower roll number (starting with 12CS):"))
up=int(input("Enter upper roll number (starting with 12CS):"))

l='12CS0'+str(low)
u='12CS'+str(up)

p=[x for x in y if x[1]>l and x[1]<u]

print(p)


##############  PRACTICAL 7 ##############

# Program to remove the i_th occurrence of the given word in a list where words repeat

List2=['python' , 'java', 'Hadoop' , 'python' , 'c' , 'python']
for I in List2:
    if I == 'python':
        List2.remove('python')

if 'python' not in List2:
    print(List2)    

##############  PRACTICAL 8 ##############
    

# Program to count the occurrences of each word in given string sentence.

string="This is a sample Python program, Welcome to World Of Python Programming!"
word="Python"
list=[]
wordCount=0
list=string.split(" ")
for i in range(0,len(list)):
    if(word==list[i]):
        wordCount+=1

print("Number of occurrences found in the string:")
print(wordCount)

##############  PRACTICAL 9 ##############

# Program to map two lists into dictionary

students = ['Shubham', 'piyush', 'sonu', 'Abhi']
marks = [89, 53, 92, 86]

students_dict = dict(zip(students, marks))
print(students_dict)

##############  PRACTICAL 10 ##############


# Program to count the frequency of word appearing in a string using a dictionary
my_string = input("Enter the string :")
my_list=[]
my_list=my_string.split()
word_freq=[my_list.count(p) for p in my_list]
print("The frequency of words is ...")
print(dict(zip(my_list,word_freq)))

##############  PRACTICAL 9 ##############

'''Program to create a dictionary with key as first character and value as words starting
with that character'''

my_string=input("Enter the string :")
split_string = my_string.split()
my_dict={}
for elem in split_string:
    if(elem[0] not in my_dict.keys()):
        my_dict[elem[0]]=[]
        my_dict[elem[0]].append(elem)
    else:
        if(elem not in my_dict[elem[0]]):
            my_dict[elem[0]].append(elem)
print("The dictionary created is")
for k,v in my_dict.items():
    print(k,":",v)
    
##############  PRACTICAL 11 ##############

# Program to find the length of a list using recursion

def list_length(my_list):
    if not my_list:
        return 0
    return 1 + list_length(my_list[1::2]) + list_length(my_list[2::2])

my_list = [26, 7, 20, 22, 40, 52, 78]
print("The list is :")
print(my_list)
print("The length of the string is : ")
print(list_length(my_list))

##############  PRACTICAL 12 ##############

# Compute the diameter,circumference,and volume of a sphere using class

import math
pi = math.pi
sphere = float(input("Enter the sphere's radius : "))
radius = sphere
diameter = 2 * radius
circumference = pi * diameter
surfaceArea = 4 * pi * radius * radius
volume = 4/3 * pi * radius * radius * radius
print("Diameter : ", diameter)
print("Circumference :",circumference)
print("surface area : ",surfaceArea)
print("volume :       ",volume)

##############  PRACTICAL 13 ##############

# Program to read file and capitalize the first letter of every word in the file

file_temp= open('python.txt', 'r')
for line in file_temp:
    Output= line.title()
    print(Output)
