Pycharm, as one of the most commonly used IDEs for Python development, is not only compatible, but also quite rich in features, such as debugging, syntax highlighting, smart prompts, etc. It also supports web development frameworks such as Django, etc. Once you are familiar with it, the development efficiency is quite high. 

![avatar]( 1e6bde0d0f68484281626f84bf30c0b8.jpg) 

 But for beginners, Pycharm is also a double-edged sword with rich features. Some small partners will inevitably be confused when they see a bunch of English interfaces just after getting started. Hahaha, it doesn't matter. Today, I will teach you 11 of Pycharm's most commonly used skills, as well as some shortcuts commonly used by pycharm, allowing you to quickly get started with Python, the most commonly used IDE in Pycharm development, and keep up with the speed of old drivers!  

###  First, common tips 

Click "File" in the upper left corner, select "Settings", enter "font" to find "Font", and set the number in "Size". The default is 12, and 18 or 20 is recommended. 

![avatar]( 911f28b9095b485d9cb44d39d6d41aa6.png) 

Here are some differences from the above. The above is to adjust the code text size, but it does not change the text size of the menu interface. If your menu interface text is relatively small, such as this: 

![avatar]( ab8ee02d893e4c0aa20b5a74cbc58927.png) 

  Then you need to adjust the text size of the menu interface. Click "File" in the upper left corner, select "Settings", enter "font", and find "Appearance". After checking in front of "Use custom font", you can choose your favorite font size in the Size at the back. 

![avatar]( fbc94d2d602249c8ab8841d8ff9b47f6.png) 

Although we can use "#" to comment on a single line of code, if there are multiple lines of code that need to be commented, it is a bit troublesome to type "#" line by line. Here we can use the mouse to select multiple lines of code, and then press Ctrl +/to comment on multiple lines of code. At the same time, we can also uncomment multiple lines of code. 

![avatar]( 883154ce0fc04884b87285f0b54bc6dc.gif) 

When we first start writing code, it is inevitable that the code will be written in an irregular manner. Although it does not affect the operation, the readability is relatively low, especially when you read a long and irregular code, you will experience the pain. 

For example, this kind of irregular spelling gives you a few spaces in the middle from time to time. 

![avatar]( a7bba2fd0eef44e18c010e4a8eb129b6.png) 

  This problem is actually very easy to solve. We just need to find "Code" in the menu bar after writing the code, and click "Reformat Code" to automatically standardize the code. 

![avatar]( c35b5bdb9aff451a8c41cefbeeeca762.gif) 

When writing code, we often have to define a lot of variables or classes. Variables or classes may be used in multiple places when writing code. If we need to modify all the variables or classes in the code, should we modify them one by one? 

Of course not, we just need to select the variable or class that needs to be renamed, right-click the pop-up option and select Refactor, and then click Rename to make global modifications. 

For example, if I want to change all "n" variables in my code to "i", then do the following: 

![avatar]( 6a938ea1173a4d209ab4ac9721e4b055.gif) 

When our code is relatively long, it is very troublesome to swipe from beginning to end to find a variable or function. At this time, we need to use the shortcut Ctrl + f to quickly find it. 

For example, I want to find out where the "runGame" function is used in the Snake project, so we just need to use Ctrl + f to bring up the small window, and then enter the keyword "runGame" to find all the places where "runGame" appears in the code. 

![avatar]( de8997afc1cf45278c5cb500a7a1c2b0.gif) 

When writing a project, it is often necessary to modify it, and sometimes it needs to be changed back and forth for several days to complete, but if we open pycharm today to add a new function, we don't want it after doing it for a long time, and we want to get back yesterday's version, but it takes a long time, and the revocation can't be pulled back. What should we do? 

At this time, you need to find the modification history. Pycharm is still very user-friendly. Every step you make changes, it saves a history for you. Just right-click the file and find all the historical versions in Local History. 

Take the simplest example, for example, my current code has an extra function to do "prompt'execution is over 'after execution is completed", I don't need it, but I can't undo it at the moment, what should I do? At this time, we can go to Local History to find the historical version and change the existing version back to the historical version. (Except for direct deletion, direct deletion is not our purpose) 

![avatar]( 89695dcb953b41d88da3c656ac76a12b.gif) 

When we use pip to install some resources, pycharm will download foreign resources for us by default. Sometimes the installation fails due to network and other problems. In fact, we can configure it and let it download domestic resources. 

The most common is to go to the open-source mirror station of Tsinghua University to download. We only need to set this up in pycharm, and it will be downloaded in China in the future. 

Setup method: click "File" in the upper right corner → click "Settings" → find "Python interpreter" under Project → click "+" → click "Manage Repositories" → click "+" → Enter the address of Tsinghua University Open Source Software Mirror Station: https://pypi.tuna.tsinghua.edu.cn/simple 

![avatar]( b100e8f14cca4c23877545e322fa5e36.gif) 

>  Fan benefits, click to view 

When writing code to implement certain functions, we often have to install packages, so it is necessary to master the function of installing packages for pycharm. 

Method: 

Click "File" in the upper left corner → click "Settings" → find "Python interpreter" under Project → click "+" → enter the name of the package you want to install, such as "pygame", and then click "Install Package" below to start the installation. After the installation is complete, you can use it. 

![avatar]( d5746ce77c9a48998bee3155934649ae.gif) 

  Note that it can only be used after the installation is completed, and there will be a download progress bar at the bottom of the interface: 

![avatar]( 3352dce2a29841d194e148fdb6b8ea33.png) 

When writing code, it is easy to report errors, but sometimes it is difficult for us to see the problem on the surface. Therefore, we need to debug at this time, which is also a commonly used technique in the development process. 

How to debug? Click on the left side of the line of code that you think may go wrong, and a red dot will appear. We call it a breakpoint. As long as the program runs to the breakpoint, it will automatically stop. After setting the breakpoint, we right-click "Debug project name" to run, and then go to the run interface. We can walk step by step and see the changes in the values of some variables inside. 

![avatar]( b9aa4bcb1c5641e6bf8e58e9d4d555a6.gif) 

There are also many ways to debug, and you can search for specific debugging skills online. I won't explain too much here. 

This is an additional function. You can set a personalized background for your pycharm, depending on your personal needs. If you want to set it, you can set it up. After all, reading English and numbers when writing code is quite tiring. Occasionally, you can also look at something else, such as your girlfriend. 

![avatar]( f2b747a612be4158bbebfb5ed3fc5ddf.png) 

  Setup method: 

① Open pycharm, click File, and select Settings. 

② Under the Appearance & Behavior option, click Appearance, click Background Image. 

③ Click on the "..." place in the upper right corner, and you can choose the picture you want to use as the background. After confirming, choose the display method you like. I think the second method is still good. 

The last thing is to set the brightness of the background image. I suggest that the brighter background should be about the same at 10% transparency. If it is too bright, it will affect the code, personal preference and picture color. 

(To clarify, that background is not mine.) 

>  Fan benefits 

###  Common shortcuts 

Finally, I will attach a summary of Pycharm's commonly used shortcuts. I wish you all the best in the process of writing code. 

![avatar]( 50716b350cc047abb58a1ba971831e4e.jpg) 

  Recently, there have been too many stolen pictures and stolen texts, so I can only add watermarks. If there is no watermark, you can chat with me privately, or you can organize some of your commonly used ones yourself. 

###  Conclusion 

I would like to advise those who are not good at English and are afraid of English software not to install the Chinese version of the development software because of this. In addition to the fact that the Chinese version does not have the native English version, the stability will be better. The biggest reason is that the vast majority of mainstream development software now uses the original English version. If you permanently use the Chinese version, you will be helpless if you encounter the English version of the software one day. 

Just like when we learn to drive, if you learn automatic transmission, then one day you will be given a manual transmission, you will not be able to drive, but if you learn manual transmission, then it is also easy to drive automatic transmission. 

![avatar]( d9935be2969b4aa9aa3fa894882d5fdc.gif) 

The Chinese version is like an automatic transmission, and the original English version is like a manual transmission. Don't be afraid just because you don't understand English at first. I'm not sampling, I'm just posting, the original version will be better, of course, there are exceptions to everything. If you learn easy language, then the Chinese version of the software is undoubtedly the best. 

![avatar]( 74456cb55762427995a2052bbc532412.png) 

