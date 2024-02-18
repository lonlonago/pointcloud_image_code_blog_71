directory 

10.1.1 understand list types 

Type name of 10.1.2 list 

Definition of 10.1.3 List 

10.1.4 Traverse Iterable Objects 

10.1.5 knowledge points 

Learn Python 10.1.6 System 

##  10.1.1 understand list types 

In our daily lives, we all come into contact with the data type "list", such as the table of contents of a book, the details of the bill at the checkout of the restaurant, the planning of the schedule, etc. The list type is a data collection that arranges the elements in the collection in order. The list type in Python is a data collection enclosed by the [] symbol, and the elements in the collection are separated by English commas. In the list type, any data type can be included: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574581220
 ```  
![avatar]( 747511447e2164c0a1cb516238055a5c.png) 

The data structure of a list is the same as that of a string, which is a linear sequential table structure. 

![avatar]( 4b99bf0a0086c1ac70d0e91dcb4a56d6.png) 

As can be seen from the figure, the list type also corresponds to a contiguous memory. 

>  Students who are not familiar with linear sequential table structures can review the content of Section 9.1, "Basic Concepts of Strings". 

In a linear sequential table structure, elements in a data collection can be accessed by indexing: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574581220
 ```  
>  Indexes in Python are numbered from 0, 0 for the first position, and 1 for the second position. Python also supports negative indices, which are numbered from -1, -1 for the penultimate position, -2 for the penultimate position, and so on. 

##  Type name of 10.1.2 list 

In interactive mode, type to output the type name of a string: 

>  >>> container = [1, '2', 3.0, True]

> >> type(container)

<class 'list'> 

From the output, the type of the list is named list. 

##  Definition of 10.1.3 List 

The list is defined by object definition and direct definition. 

(1) Object definition method 

The type name of the list is list, and you can directly execute help (list) in interactive mode to find the definition and usage of list: 

>  >>> help(list)

Help on class list in module builtins:

class list(object)

|  list(iterable=(), /)

|

|  Built-in mutable sequence.

|

|  If no argument is given, the constructor creates a new empty list.

|  The argument must be an iterable if specified. 

In the output of interactive mode, the form of list (iterable = (),/) is the object definition method. The parameter iterable represents an iterable object. Among the data types learned so far, string and list are both iterable objects. In Python, any data type that can iterate over the elements in the collection is an iterable object. The so-called traversal is to access the elements in the collection one by one. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574581220
 ```  
(2) Direct definition method 

The so-called direct definition method is to define a list directly through the [] symbol: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574581220
 ```  
List types can contain any data type, and now nested lists are defined by direct definition. The so-called nested list refers to the inclusion of a list in a list. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574581220
 ```  
We usually see pictures, tables, etc. as a two-dimensional data structure. 

##  10.1.4 Traverse Iterable Objects 

The simple data types in Python are all non-iterable objects. The simple data types learned so far are integers, floating-point types, and boolean types. Composite data types in Python are all iterable objects. For iterable objects, you can iterate over the elements in the collection in the for loop structure. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574581220
 ```  
##  10.1.5 knowledge points 

>  (1) A list type is a collection of data that arranges the elements in the collection in order

(2) In Python, the list type enclosed by [] is used, and the elements in [] are separated by English commas

(3) The type name of the list is list, and like string, the list is also a linear sequence structure

(4) Lists can be defined by object definition and direct definition

(5) Simple data types are non-iterable, and composite data types in Python are all iterable objects

(6) For iterable objects, you can iterate through the elements in the collection in a for loop 

##  Learn Python 10.1.6 System 

>  About the French fries teacher: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. French fries teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 

