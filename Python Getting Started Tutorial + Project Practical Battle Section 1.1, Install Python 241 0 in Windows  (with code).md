directory 

1.1.1 install Python in Windows 

1.1.2 system to learn Python 

##  1.1.1 install Python in Windows 

When learning the Python programming language, you need to install the Python interpreter first. 

>  Readers must be familiar with language translators. We use translators to translate Chinese into English, so that foreign friends can understand the meaning of Chinese expressions. A Python interpreter is also a translator that translates Python programs into machine instructions that a computer can execute. 

The development environment in which the author is located is a 64-bit Windows 10 system. Please follow the steps below to install the latest stable version of the Python interpreter in the Windows environment step by step. 

(1) Download the Python installation package 

Open the official Python website Welcome to Python.org, you can see a Downloads navigation menu on the page. Select Windows in the Downloads submenu, and then click Python 3.X on the right side of the page (X represents the corresponding version number, the version I installed is 3.11.0) to start downloading the latest Python installation package: 

![avatar]( 57954ad0e6c4f3dcbec9b7f796f7d0c5.png) 

​ 

(2) Python installation options 

After downloading the installation package to the local area, click the right mouse button to run the downloaded Python installation package as an administrator. The reason why you need to run as an administrator is that you need to configure the environment information during the installation process, which requires administrator privileges. 

![avatar]( 7da92737d3ceb4df873c128edcf8de30.png) 

​ 

![avatar]( 754361c1e043d0e8e6a61e0940510a91.png) 

​ 

>  ① The Install Now option means to install directly according to the default configuration of Python, usually according to the default configuration. ② The Customize installation option means to customize the installation path of Python and tick the Python features you need. 

Students need to check Add python.exe to PATH before clicking the Install Now button. The purpose of checking this item is to add the Python interpreter to the system environment variables PATH of Windows. 

![avatar]( 9db3991c492b3d0e6773fc4869abfd1c.png) 

After adding the Python interpreter to the environment variables PATH, you can execute Python scripts directly from the Windows command line. 

>  The so-called environment variables are a series of parameters of the system operating environment, such as the system environment variables PATH here, which saves parameters related to the path. The system searches for the path saved by PATH in the path search. 

(3) Click the install Now button to install Python 

![avatar]( 62462856a29a9a91b60f5041283438bd.png) 

(4) Test whether Python is installed successfully 

Press the windows key of the keyboard, then enter the cmd command and press the enter key to enter the command line interface of windows. Execute the python -V command in the command line interface of windows. If the relevant output of the Python version appears, the installation is successful: 

![avatar]( 66cbb6a4d7888159d297e9ef3bc84f20.png) 

>  Students need to note that a space should be added between python and -V, -is an underscore, and V is an uppercase V. 

##  1.1.2 system to learn Python 

>  Fries Teacher Profile: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. Fries Teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning 

