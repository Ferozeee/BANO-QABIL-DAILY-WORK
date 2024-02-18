# python -m pip install plotly
import plotly.express as px

df = px.data.gapminder()

fig = px.bar(df, x="continent", y="pop", color="continent",
  animation_frame="year", animation_group="country", range_y=[0,4000000000])
fig.show()
import streamlit as st

# Using object notation
add_selectbox = st.sidebar.selectbox(
    "How would you like to be contacted?",
    ("Email", "Home phone", "Mobile phone")
)

# Using "with" notation
with st.sidebar:
    add_radio = st.radio(
        "Choose a shipping method",
        ("Standard (5-15 days)", "Express (2-5 days)")
    )
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
   
class Employee:
    def __init__(self, name, emp_id, salary, department):
        self.name = name
        self.id = emp_id
        self.salary = salary
        self.department = department

    def calculate_salary(self, salary, hours_worked):
        overtime = 0
        if hours_worked > 50:
            overtime = hours_worked - 50
        self.salary = self.salary + (overtime * (self.salary / 50))

    def assign_department(self, emp_department):
        self.department = emp_department

    def print_employee_details(self):
        print("\nName: ", self.name)
        print("ID: ", self.id)
        print("Salary: ", self.salary)
        print("Department: ", self.department)
        print("----------------------")


employee1 = Employee("ADAMS", "E7876", 50000, "ACCOUNTING")
employee2 = Employee("JONES", "E7499", 45000, "RESEARCH")
employee3 = Employee("MARTIN", "E7900", 50000, "SALES")
employee4 = Employee("SMITH", "E7698", 55000, "OPERATIONS")

print("Original Employee Details:")
employee1.print_employee_details()
employee2.print_employee_details()
employee3.print_employee_details()
employee4.print_employee_details()

# Change the departments of employee1 and employee4
employee1.assign_department("OPERATIONS")
employee4.assign_department("SALES")

# Now calculate the overtime of the employees who are eligible:
employee2.calculate_salary(45000, 52)
employee4.calculate_salary(45000, 60)

print("Updated Employee Details:")
employee1.print_employee_details()
employee2.print_employee_details()
employee3.print_employee_details()
employee4.print_employee_details()

import datetime
import streamlit as st

d = st.date_input("When's your birthday", datetime.date(2000, 7, 6))
st.write('Your birthday is:', d)

import pandas as pd
import streamlit as st

data_df = pd.DataFrame(
    {
        "apps": [
            "https://storage.googleapis.com/s4a-prod-share-preview/default/st_app_screenshot_image/5435b8cb-6c6c-490b-9608-799b543655d3/Home_Page.png",
            "https://storage.googleapis.com/s4a-prod-share-preview/default/st_app_screenshot_image/ef9a7627-13f2-47e5-8f65-3f69bb38a5c2/Home_Page.png",
            "https://storage.googleapis.com/s4a-prod-share-preview/default/st_app_screenshot_image/31b99099-8eae-4ff8-aa89-042895ed3843/Home_Page.png",
            "https://storage.googleapis.com/s4a-prod-share-preview/default/st_app_screenshot_image/6a399b09-241e-4ae7-a31f-7640dc1d181e/Home_Page.png",
        ],
    }
)

st.data_editor(
    data_df,
    column_config={
        "apps": st.column_config.ImageColumn(
            "Preview Image", help="Streamlit app preview screenshots"
        )
    },
    hide_index=True,
)





    
