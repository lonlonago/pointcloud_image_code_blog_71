directory 

1.2.1 Linux system classification 

1.2.2 install Python on Linux systems 

1.2.3 system to learn Python 

###  1.2.1 Linux system classification 

In the Python official website also provides the installation package for the Linux system. In the main distribution of the Linux system, it can be divided into Deb system and RPM system according to its software package format. Linux system and Windows system have a very important difference: Linux system is completely free and open source, while Windows system is paid and closed source. In enterprises, Linux system is usually used as a server. Deb system is more representative of Ubuntu and Debian. Ubuntu is mainly used as a desktop operating system, Debian is used as a server operating system. 

![avatar]( 1925dd5c0d5c01442884019c0ed67d1b.png) 

![avatar]( ed5508da657be5c29a6d75384148690a.png) 

The RPM system is mainly used as a server operating system, and the more representative ones are Redhat and CentOS. 

![avatar]( 5286d702f346c3f77b8116f60abfe437.png) 

![avatar]( e458d27c8a176aabf438d2785f78059e.png) 

​ 

>  Beginners who are interested in Linux systems can create a virtual machine in the Windows system through tools such as VMware or VirtulBox, and then download the image file of the Linux system to run Linux system in the virtual machine. 

##  1.2.2 install Python on Linux systems 

In this tutorial, the author takes the CentOS system in the RPM department as an example to demonstrate how to install python in the Linux. Students should note that this is only to explain how to install the Python interpreter in the Linux system. For beginners, it is most convenient to learn Python directly using the Windows system. Regarding the installation of the Python interpreter, please follow the steps below: 

(1) Download the python source package 

Open the Python source package download page: Python Source Releases | Python.org 

![avatar]( 7a63a81c460ee686e01fc5e597d3c8e2.png) 

Click the Latest Python 3 Release link to enter the python source package download page. Slide down to the bottom of the page in the download page, and then directly click the Gzipped source tarball link to download the python source package in gzip format: 

![avatar]( 81cbf790b6c4b0e27210354787a1a9a2.png) 

In Linux system, you can also download the source code package of python3 directly from the command line through the wget command. Download link of Python source code package: https://www.python.org/ftp/python/3.7.4/Python-3.7.4.tgz 

Usage of downloading using the wget command: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574572722
 ```  
If you need to download other versions of python, you can directly replace the version number in the link, for example, download python 3.5.1: https://www.python.org/ftp/python/3.5.1/Python-3.5.1.tgz 

(2) Unzip the Python source package 

Upload the gzip archive to your Linux system via tools such as FTP, and then use Linux tar command to unzip it. 

The compressed package file downloaded by the author is Python-3.7.4, and the decompression command is: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574572722
 ```  
The decompressed directory is Python-3.7.4, execute the cd Python-3.7.4 command on the command line to enter the source directory. 

The directory structure is as follows: 

![avatar]( dc4af6bdc47a053bb80e9d13caeda6d8.png) 

>  Beginners need to be familiar with the Linux system and will use common commands. For example, the "ls" command in the screenshot is actually the abbreviation of the English word "list", which means "list". For more meanings and usage of the ls command, readers can consult the official documentation or make good use of search engines. Linux configure and make. Configure is a script configuration tool in Linux, which is used to detect the current installation environment of the source code. If the detection is correct, it will generate a Makefile script file for source code compilation in the current directory. Make is a compilation and installation tool under the Linux system, which is used to explain the compilation and installation commands in the makefile file. 

(3) Generating Python Makefiles 

Executing./configure in the current directory Python-3.7.4 generates a Makefile file. 

>  When using the configure command to generate a Makefile file, you can specify the --prefix parameter to specify the installation directory of python. The syntax is --prefix = "the path of your custom installation directory". If this parameter is not specified, then the default installation path of python in linux is/usr/local. The rules for compiling, linking and installing the source program are defined in the Makefile file, and the project source program can be automatically compiled through the Makefile file. 

Output after executing the configure command: 

![avatar]( 595558430bb412fd127fa8f2578b0b7e.png) 

​ 

(4) Compiling Python 

After the configure command ends, a Makefile file will be generated in the current directory, and then enter the make command source code to compile Python. The command output is shown in the following figure: 

![avatar]( 2bd4a76d39d86b2d41b5cb6c853ea6c6.png) 

(5) Install Python 

After the compilation is successful, execute the sudo make install command to start installing python. If no installation directory is specified, the default installation directory is/usr/local, and the corresponding python interpreter is installed in the/usr/local/python3/bin directory. After the installation is completed, execute/usr/local/python3/bin/python3.7 -V on the command line to see the version information of python. 

![avatar]( 855f20e3bb6a758f74a69b6ad97bd0ca.png) 

(6) Set up soft links 

The installed python can be executed by means of an absolute path, such as/usr/local/python3/bin/python3.7 in step 6. It is troublesome to execute python by typing a large path each time. In the Linux system, you can set a soft link for the installed python. The soft link here is similar to the file shortcut of the Windows system. Execute the following command to set a soft link for python: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574572722
 ```  
>  In the ln command, it is a soft link that sets the path on the left to the path on the right. The/usr/bin directory has been added to the Linux environment variables PATH, so executing python3 is equivalent to executing/usr/bin/python3. 

Pip is a package management tool for python, execute the following command to set up soft links for pip: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574572722
 ```  
>  When introducing module management in Python later, we will explain pip in detail. 

##  1.2.3 system to learn Python 

>  Fries Teacher Profile: Senior technical expert, technical writer, author of "Python Zero Basic Introduction Guide", "Java Zero Basic Introduction Guide" and other technical tutorials. Fries Teacher's blog: http://www.chipscoco.com, system learning backend, crawler, data analytics, machine learning 

