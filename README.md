# list with elements of different data types
list1 = [5, "Hello", 9.4]
print (list1)

# List slicing in Python

my_list = ['p','r','o','g','r','a','m','i','z']

# items from index 2 to index 4
print(my_list[0:9])

# items from index 5 to end
print(my_list[5:6])

# items beginning to end
print(my_list[:])

numbers = [21, 34, 54, 12]

print("Before Append:", numbers)

# using append method
numbers.append(32)

print("After Append:", numbers)

languages = ["Python", "Swift", "C++"]

# access item at index 0
print(languages[-1])   # C++

# access item at index 2
print(languages[-3])   # Python

numbers = [1, 3, 5]

even_numbers = [4, 6, 8]

# add elements of even_numbers to the numbers list
numbers.extend(even_numbers)

print("List after append:", numbers)


languages = ['Python', 'Swift', 'C++', 'C', 'Java', 'Rust', 'R']

# deleting the second item
del languages[1]
print(languages) # ['Python', 'C++', 'C', 'Java', 'Rust', 'R']

# deleting the last item
del languages[-1]
print(languages) # ['Python', 'C++', 'C', 'Java', 'Rust']

# delete the first two items
del languages[0 : 2]  # ['C', 'Java', 'Rust']
print(languages)

languages = ['Python', 'Swift', 'C++', 'C', 'Java', 'Rust', 'R']

languages = ['Python', 'Swift', 'C++', 'C', 'Java', 'Rust', 'R']

# remove 'Python' from the list
languages.remove('Python')

print(languages) # ['Swift', 'C++', 'C', 'Java', 'Rust', 'R']


languages = ['Python', 'Swift', 'C++', 'C', 'Java', 'Rust', 'R']

# deleting the second item
del languages[1]
print(languages) # ['Python', 'C++', 'C', 'Java', 'Rust', 'R']

# deleting the last item
del languages[-1]
print(languages) # ['Python', 'C++', 'C', 'Java', 'Rust']

# delete the first two items
del languages[0 : 2]  # ['C', 'Java', 'Rust']
print(languages)

languages = ['Python', 'Swift', 'C++']

# iterating through the list
for language in languages:
    print(language)

languages = ['Python', 'Swift', 'C++']

print('SQRL' in languages)    # False
print('Python' in languages)    # True

languages = ['Python', 'Swift', 'C++']

print("List: ", languages)

print("Total Elements: ", len(languages))    # 3

# create a list with value n ** 2 where n is a number from 1 to 5
numbers = [n**2 for n in range(1, 6)]

print(numbers)    

# Output: [1, 4, 9, 16, 25]

# create a list
numbers = [2, 3, 5, 2, 11, 2, 7]

# check the count of 2
count = numbers.count(2)


print('Count of 2:', count)

#Class example no 1
# define a class
class Bike:
    name = ""
    gear = 0

# create object of class
bike1 = Bike()

# access attributes and assign new values
bike1.gear = 11
bike1.name = "Mountain Bike"

print(f"Name: {bike1.name}, Gears: {bike1.gear} ")

# Python3 program to
# demonstrate instantiating
# a class
class Human:
	# A simple class
	# attribute
	attr1 = "human"
	attr2 = "student"

	# A sample method
	def fun(self):
		print("I'm a", self.attr1)
		print("I'm a", self.attr2)
# Driver code
# Object instantiation
Rodger = Human()

# Accessing class attributes
# and method through objects
print(Rodger.attr1)
Rodger.fun()

class Python:
	def __init__(self, name, company):
		self.name = name
		self.company = company
	def show(self):
		print("Hello my name is " + self.name+" and I" +
			" work in "+self.company+".")
obj = Python("ALI ABBAS", "N.G.V.S.")
obj.show()

#class example no 2
class students:
    name = ""
    Id = ""
    phone = ""
    
#creat objects of class
student1 = students()

student1.name = input("Enter student name : ")
student1.Id = int(input("Enter student Id : "))
student1.phone = int(input("Enter student phone no  : "))

print(f"Name: {student1.name}, Id no: {student1.Id}, Phone no: {student1.phone}")  


import math

a = math.sqrt(49)
b = math.ceil(2.8)
c = math.floor(2.8)
d = math.pi
import datetime
e = datetime.datetime.now()

print(a)
print(b)
print(c)
print(d)
print(e.year)
print(e.strftime("%A"))

#Declaring a function
def fun():
     print("Name: Ali Abbas")
     print("F.Name: Abdul Latif")
     print("Campus: Daftar-e-Jamat Islami korangi")
     print("cell no: 03112074782")
     print("Gmail: aliabbas02022006@gmail.com")
    #Driver's code
    #Calling fun
fun()

def evenodd(f):
    if (f % 2 == 0):
        print("even")
    else:
        print("odd")
        
    #Driver's code
evenodd(234)
evenodd(365)

# python programming
# default arguments
def myfun(x, y = 50):
    print("x: ", x)
    print("y: ", y)
myfun(43)    

#keywords Arguments
def student(firstname, lastname):
    print(firstname, lastname)

student(lastname = 'Abdul Latif', firstname='Ali Abbas')

ages = {"ali":18,"saqib":24}
del ages ["saqib"]
print(ages)
   










    
