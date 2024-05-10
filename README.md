# Python-Collection-Data-Types (List,Tuples,Dictionary & Sets)
    
     1.Lists
     2.Tuples
     3.Dictionary
     4.Sets


#  1.Lists:
       • Mutable
       • To hold sequence of values like Age, Gender etc
       • To create lists we need square brackets - []
       • collection items of multiple datatypes


# 1. 

marks = [11,22,33,44,55,66,77,88,99]
print(type(marks))


# 2. 

language = [['English','Hindi'],'Sanskrit',['Math','Science'],['History','Geography'],'Python']
print(language[0])
print(language[0][1])
print(language[2])
print(language[2][1])
print(language[2][0])
print(type(language[1]))
print(type(language[2]))



# list data type:

list = ['Rakesh',True,12.9,45]
print(type(list))   #<class 'list'>
print(type(list[0]))  #<class 'str'>
print(type(list[1]))  #<class 'bool'>
print(type(list[2]))  #<class 'float'>
print(type(list[3]))  #<class 'int'>



# List Updation:

list = [20,30,10,90,89,76]
list[1]=11
list[2]=12
print(list)

list[0:5] = [11,22,33,44,55,66]
list[0:2] =['Ramesh',True,22.45]
print(list)



# Append Method: 
        •Can be a single value or a list, list will append as list of list


marks = [33,45,67,89,98]
marks.append(70)
print(marks)


# Or.

Name = ['AAA','WWW','QQQ']
Name.append('Numbers')
print(Name)'''

# Or.

Name = ['AAA','WWW','QQQ']
Name.append(['Numbers','Mahesh',12])
print(Name)



# CLEAR Method:

Name = ['AAA','WWW','QQQ']
Name.clear()
print(Name)



# Copy Method: 
        •A new copy created


Name = ['AAA','WWW','QQQ']
Name = Name.copy()
print(Name)




# COUNT Method: 
        •That means if 11 is written three times in the list below then the output will also be 3.


Number = [11,33,55,11,77,11,99,67]
c= Number.count(11)
print(c)




# Extend Method:
           •Always be a list but save as individual elements



Number = [11,33,55,11,77,11,99,67]
Number.extend([10,20,30,40,50])
print(Number)


# Or.

Number = [11,33,55,11,77,11,99,67]  # no. of index position
i = Number.index(77)
print(i)





# Insert Method:
         •Insert the records at any position using index


Number = [11,33,55,11,77,11,99,67]
Number.insert(4,100)
print(Number)



# Pop method:
       •Pop removes the last value from the list if index not provided. 
        Else, it will remove the value of the index provided.



Number = [11,33,55,11,77,11,99,67]
Number.pop()
# Number.pop()
# Number.pop()
Number.pop(3)
print(Number)




# Remove Method:
            •Remove removes the value given in the command


n = [11,33,55,11,77,11,99,67]
n.remove(99)
#n.remove(67)
print(n)




# Reverse Method:
         •Just reverse the list, no sorting



Number = [11,33,55,11,77,11,99,67]
Number.reverse()
print(Number)



# Sort Method:
         •Sort ascending order



Number = [11,33,55,11,77,11,99,67]
Number.sort()
print(Number)



# sum :

Number = [11,33,55,11,77,11,99,67]
s = sum(Number)
print(s)






# 2. Tuple:
    
     • Tuple are immutable, i.e., they can't be changed
     • Tuple are faster than list
     • Tuples are used to store multiple items in a single variable.
     • Tuples are written with round brackets ().
     • collections of heterogeneous.(Tuples are a sequence of data of different data types 
       (like integer, float, list, string, etc;) and can be accessed through indexing and slicing.)

      • Contains duplicate: Allows duplicates data.



tuple = ("apple", "banana", "cherry")
print(tuple)


# Or.

record = ("John", 35, "Python Developer")
print(record)



# We use index numbers to access tuple items. For example,



languages = ('Python', 'Swift', 'C++')

# access the first item
print(languages[0])   # Python

# access the third item
print(languages[2])   # C++




# We use the len() function to find the number of items present in a tuple. For example,


cars = ('BMW', 'Tesla', 'Ford', 'Toyota')
print('Total Items:', len(cars))





# We use the for loop to iterate over the items of a tuple. For example,



fruits = ('apple','banana','orange')

# iterate through the tuple
for fruit in fruits:
    print(fruit)






# 3. Dictionary:
        • Dictionary are used to store data value in key : value Pairs.
        • Unordered: The items in dict are stored without any index value.
        • Unique: Keys in dictionaries should be Unique.
        • Mutable: We can add/Modify/Remove key-value after the creation.



dict1 = {'cust_id':[1,2,3,4,5],'cust_name':['A','B','C','D','E'],'region':['N','S','S','E','W']}
#print(dict1)
dict1['product'] = ['TV','Freeze','iron','Tubelight','AC']
# print(dict1)
# dict1['cust_name'][0] = 'Z'  #update cust_name
# print(dict1)
dict1.clear()
print(dict1)




# Or.

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
        


# Or.



Dict = {1: 'Namak', 2: 'haldi', 3: 'Ghee'}
print(Dict)



# We can access the value of a dictionary item by placing the key inside square brackets.



country_capitals = {
  "Germany": "Berlin", 
  "Canada": "Ottawa", 
  "England": "London"
}

# access the value of keys
print(country_capitals["Germany"])    # Output: Berlin
print(country_capitals["England"])    # Output: London




# We can add an item to a dictionary by assigning a value to a new key. For example,




country_capitals = {
  "Germany": "Berlin", 
  "Canada": "Ottawa", 
}

# add an item with "Italy" as key and "Rome" as its value
country_capitals["Italy"] = "Rome"

print(country_capitals)




# import pandas:


import pandas
mydataset = {
  'cars': ["BMW", "Volvo", "Ford"],
  'passings': [3, 7, 2]
}
myvar = pandas.DataFrame(mydataset)
print(myvar)








# 4. Set:
     •Unordered: Set doesn't maintain the order of the data insertion.
     •Unchangeable: Set are immutable and we can't modify items.
     •Heterogeneous: Set can contains data of all types
     •Unique: Set doesn't allows duplicates items




myset = {1,2,2,1,3,3,4,5,4,5}
#print(myset)
myset.add(100)
myset.add(200)
#myset.clear()
# myset.pop()
#myset.remove(3)
myset.update({11})
print(myset)




# .


# create a set of integer type
student_id = {112, 114, 116, 118, 115}
print('Student ID:', student_id)

# create a set of string type
vowel_letters = {'a', 'e', 'i', 'o', 'u'}
print('Vowel Letters:', vowel_letters)

# create a set of mixed data types
mixed_set = {'Hello', 101, -2, 'Bye'}
print('Set of mixed data types:', mixed_set)







# Creating an empty set is a bit tricky. Empty curly braces {} will make an empty dictionary in Python.
      To make a set without any elements, we use the set() function without any argument. For example,





# create an empty set
empty_set = set()

# create an empty dictionary
empty_dictionary = { }

# check data type of empty_set
print('Data type of empty_set:', type(empty_set))

# check data type of dictionary_set
print('Data type of empty_dictionary:', type(empty_dictionary))




# Let's see what will happen if we try to include duplicate items in a set.


numbers = {2, 4, 6, 6, 2, 8}
print(numbers)   # {8, 2, 4, 6}
