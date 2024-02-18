directory 

Common Operators in 10.2.1 Lists 

10.2.2 [] operator: index access list 

10.2.3 [:] operator: slice of list 

10.2.4 + operator: addition of lists 

10.2.5 * operator: multiplication of lists 

Relational operations 10.2.6 lists 

10.2.7 in operator: find element 

10.2.8 knowledge points 

Learn Python 10.2.9 System 

##  Common Operators in 10.2.1 Lists 

List type is an abstract data type. Abstract data type defines the operation method of the data type. In this section, we focus on manipulating lists through operators. 

![avatar]( d26c7f83a3ff2b323348f6cbd0b3e81a.png) 

The commonly used operators for list types are shown in the following table: 

![avatar]( 9d50ad2b32f3befcab891ac7919509b5.png) 

##  10.2.2 [] operator: index access list 

In Section 9.2, we introduced how to access the characters in a string through an index. The list type is also a linear sequence structure, and like a string, you can access the elements of the list through an index. 

Operation syntax: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574567984
 ```  
String is a static data type that can only be read by indexing characters and cannot be modified. The list type can be modified by indexing elements. 

Indexes in Python are divided into positive and negative indices. Positive indices are numbered from 0 and represent the first element in the data set. Negative indices are numbered from -1 and represent the first to last element in the data set. Positive and negative index values must be within a valid range or an out-of-bounds access error message will be thrown. Students who are not familiar with this can review the content in Section 9.2. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574567984
 ```  
Variables in Python actually store the memory address. When assigning a list to another variable, the memory address of the list is actually assigned. After the assignment operation is completed, modifying the variable will affect the original list. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574567984
 ```  
For the above code example, students can understand it through the following figure. The numbers variable holds the address of the list in memory. 

![avatar]( 2fc168d3efe8d9e6ccee0dae5fb110fe.png) 

After assigning the variable numbers to the variable container, both the variable container and the variable numbers refer to the same list. 

![avatar]( ecd496c13f2c9200318b714cf6066a82.png) 

Students can verify in interactive mode and use id to output the memory address of the variable: 

> >> numbers = [1,2,3,4]

> >> container = numbers

> >> id(numbers)

2890924839944

> >> id(container)

2890924839944 

This assignment feature of lists is also known as shallow copying. Shallow copying refers to copying memory addresses. As opposed to shallow copying, deep copying copies all the data in memory to the new memory space. After deep copying, it does not affect the original data object. When assigning values to composite data types in Python, shallow copying is performed. 

##  10.2.3 [:] operator: slice of list 

The trimming operation syntax is the same as the string slicing operation. For those who are not familiar with this, please review the content in Section 9.2. After slicing the list, a new list is returned. 

Operation syntax: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574567984
 ```  
Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574567984
 ```  
##  10.2.4 + operator: addition of lists 

List addition is the process of combining elements from two lists into a new list. 

Operation syntax: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574567984
 ```  
Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574567984
 ```  
##  10.2.5 * operator: multiplication of lists 

The "*" operator is used to repeatedly output a list and return a new one. 

Operation syntax: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574567984
 ```  
The parameter number must be an integer number. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574567984
 ```  
##  Relational operations 10.2.6 lists 

Use relational operators to perform a relational operation on a list and return a result of type Boolean. 

Operation syntax: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574567984
 ```  
Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574567984
 ```  
The relational operation of a list is an ordered comparison, where the ordered comparison starts from the first element of the list and is compared element by element. 

>  The two lists are equal only if the element values are the same and the order is the same. Otherwise, the size relationship of the list is determined by the size relationship of the element sequence. 

For example, in the code above, although the list right has only one element, the first element in right is greater than the first element in the list left. At this time, Python will directly determine that the list right is greater than the list left, even if the elements behind the list left are larger than the elements in the list right. Now the relationship operation of the list is simulated through the loop structure. 

Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574567984
 ```  
##  10.2.7 in operator: find element 

Use the "in" operator to determine whether an element exists in the list, and return a boolean value of True if present, False otherwise. 

Operation syntax: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574567984
 ```  
When indicating whether it does not exist, it needs to pass the logical NOT operator not: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574567984
 ```  
Code example: 

Python 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574567984
 ```  
##  10.2.8 knowledge points 

>  (1) A list type is a linear sequence structure that allows access to elements in a list through an index.

(2) String is a static data type that can only be read by indexing characters and cannot be modified. List types can be modified by indexing elements.

(3) Variables in Python store memory addresses. When assigning a list to other variables, the memory address of the list is actually assigned. After the assignment operation is completed, modifying the variable will affect the original list.

(4) Assignment to composite data types in Python is performed by shallow copying.

(5) The relationship operation of the list is to compare in order. The order comparison here starts from the first element of the list and compares element by element. Only if the element values are the same and the order is the same, the two lists are equal. Otherwise, the size relationship of the list is determined by the size relationship of the elements. 

##  Learn Python 10.2.9 System 

>  About the French fries teacher: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. French fries teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning, quantitative investment. 

