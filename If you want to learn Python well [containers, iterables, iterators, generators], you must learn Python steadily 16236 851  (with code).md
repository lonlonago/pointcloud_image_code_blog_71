When I first started learning Python, did I often hear bosses talking about containers, iterables, iterators, generators, lists/sets/dictionary derivations, and many other concepts? In fact, this is not because the bosses just put the technical terms to install B, but these things have to be understood. It is not enough to know the basics of strings, lists, etc., especially in Python's data structures. 

![avatar]( 2ba410ec78c64b2d96bcfd183fac5018.jpg) 

Today, let's talk about the difficult concepts of containers, iterables, iterators, and generators in Python, and take your Python foundation to the next level! 

###  Container 

In Python, a container is a data structure that organizes multiple elements together, and the elements in the container can be obtained one by one iteratively. To put it bluntly, its function is just like its name: to store things (data). 

The container does not actually exist. It is not a data type, but an artificial concept. It is just a concept word created for the convenience of learning. It can use the membership operator (in or not in) to determine whether the object is in the container. 

Of course, it wasn't created by me, I don't have that much ability, it was officially created, well, don't worry, I'm teaching you some weird nouns, and no one will understand it when you say it... It's called that in python. 

![avatar]( 4e65de7e7d4f41eba25846e6ef57e294.jpg) 

Common container types include lists, tuples, strings, dictionaries, and sets. 

Since the data in the container can be obtained iteratively, we have to learn a new concept: iterable objects. 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

###  Iterable objects 

In Python, an iterable object doesn't refer to a specific data type, it refers to a container object that stores elements. 

That is to say, if there is no data stored in the container, it is not an iterable object, and not all containers are iterable objects. Containers contain but are not limited to iterable objects. 

Pay attention to two points: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
Have you ever thought about how the for loop is implemented internally? For example, in this example of a for loop, why can every element in the list be output? How is it implemented internally? 

![avatar]( b9a028d2f0454756b484ffe84a77aed8.png) 

In fact, the loop does two things: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
Then we don't need a for loop to output each element in the list, 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
Output result: 

![avatar]( a93739168dcb443a916dc1db33f9371f.png) 

It can be seen that if we remove the line of code that prints ite, the execution effect is the same as each element in the output list of the for loop. The for loop defines the range 4 times, and actually executes 1 __iter__ () and 4 __next__ (), that is to say, the essence of the for loop accessing the iterative object is achieved through this. 

Moreover, the two things that the for loop essentially does are indispensable, that is to say, if there is no __iter__ () to return the iterator first, __next () __ cannot get the element, which just shows the second point of the two points mentioned above: an iterable object cannot be iterated independently. 

There are two built-in functions that have the same principle as them and are essentially the same. It is more convenient to use built-in functions if you want to use them, at least you don't need to write so many underscores: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
![avatar]( 2fc205b9d56e48858355262021fb2e33.png) 

It can be seen that the result is exactly the same. Since iterators are mentioned, let's take a look at what an iterator is. 

![avatar]( 511a9cb2757f46879097683afe530fd4.jpg) 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

###  Iterator 

From the example of the for loop above, we can probably see that, 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
Since this is the case, when we learned the basics of Python, we said that range () is an iterable object, so it can also generate an iterator by __iter__ (). 

![avatar]( d71df4ed7b2048f68c209a8a306bfe92.png) 

###  IV. Sequence 

Sequence is also an abstract concept, which includes lists, tuples, and strings. It does not exist in itself, and is also a concept created for learning. 

Iterable objects contain sequences, and since sequences contain lists, tuples, and strings, as in our previous example, sequences can be used by iter () and next (). 

Sequences can be divided into finite sequences and infinite sequences. Finite sequences have a range, for example, range (10) has defined the range, on the contrary, infinite sequences are sequences without a limited range. 

We need to generate an infinite sequence. Here, we need to use a new module, itertools, which is a collection of iterative functions for efficient loops. It has a method count () below it, which can generate an iterator without range, which can be understood as an infinite iterator. 

![avatar]( 9fdbeb032c7c4ef69f03b4769ba78be3.png) 

From this example, we can see that as long as it is executed once, next () will fetch the contents of the iterator once and retrieve them one by one. I have only written four next () here, and you will output a few more times if you write more. 

A mechanism like next () that needs to be called when is called lazy loading mechanism, also known as lazy loading; 

On the contrary, there is hungry loading. For example, the for loop will fetch all the objects in the iterator as soon as it is executed. 

###  List derivation 

List derivation is related to the generator. Before talking about the generator, you need to know what a list derivation is. A list derivation is a method of generating a list. The syntax is as follows: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
I represents the object to be placed in the list, and the for loop is an expression. 

For example, let's use a list derivation to generate a list. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
Using list derivation can easily generate the list we want. 

And there's lots of other flexible uses of it, like conditional judgment. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
If the following condition is determined to be true, the list can be generated normally. If it is false, the list derivation is invalid. At this time, l will be an empty list. 

There are other flexible uses, such as manipulating the previous i, such as doubling the value of i: 

![avatar]( 474e4417244c4665bef84250e73e54e4.png) 

We replace the iteration object with a string, which can also be output, but * represents the repeating operator in the string, so the effect becomes like this: 

![avatar]( 07b3e0047f2b4077a4ce120d75691783.png) 

Not only that, but we can also use functions to operate the previous i * 2, such as: 

![avatar]( 1639088b00854f39ac6102409066b1de.png) 

Overall, list derivations are a flexible way to quickly and customize the generation of lists. 

Then someone may draw inferences. List derivations are all operated with [], so if you use () to operate, will it generate a tuple? Let's take a look: 

![avatar]( 5e0763154370477bb3c97164bd8ee3f8.png) 

[] 换成（）之后，返回的是一个生成器generrator ，那么下面我们再来讲讲生成器： 

###  Generator 

Generators are objects that actually exist in Python, unlike containers, which can be called directly through next (). 

The first creation method is similar to the list derivation, that is, [] is replaced by (): 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
For example, let's generate a generator and see if we can call it directly with next (): 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
It can be seen that the generator can be called directly. So since the generator can be called by next (), then the generator is a special iterator, an iterable object. 

In addition to creating a generator in the above method, you can also create it with yield as follows: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
For example, let's create a generator with a function containing yield: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
The result is a generator, and at this point the function fun () is no longer a function, it is a generator, and as long as yield appears in the function, the function becomes a generator. 

Why doesn't the while loop keep executing? Don't worry, let's output it: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
Run result: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
I called it three times, so it ran three times. The while loop exists, but it doesn't work because of the lazy loading we mentioned earlier. 

When you need it, when you use the next () call, it is lazy loading, unlike hungry loading, which generates all objects in advance. If you replace it with a for loop to complete, for example: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563625
 ```  
After running the program will enter an infinite loop, has been to add 1 to a, you can try to see the effect, that is, hungry Han type loading generates an iterator in advance and calls all iterator objects, hungry Han type loading takes up resources magnifying glass. 

![avatar]( 385b2f18574c4a5bb436f40621643d11.jpg) 

###  Summary 

The content of today's talk may sound boring, and there is nothing you can do about it. Some things may be a little "hard to swallow" for the first time. After seeing a lot, you will get used to it. You have to force yourself to try to accept and understand these abstract things. 

Finally, a diagram summarizes their relationship: 

![avatar]( 29bc787a17c4476aba3d2b5a092fa4e9.jpg) 

Well, today's sharing will stop here first. The article is written in a hurry. If there is anything not in place, please criticize and point it out. See you next time! 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

![avatar]( 9413cbb8567a4bb7a71378b8fa471832.png) 

