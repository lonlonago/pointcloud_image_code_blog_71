I don't know if you have noticed when crawling data with crawlers. More and more websites have their own anti-crawling mechanisms, and crawling data is not as easy as it used to be. The current common anti-crawling mechanisms mainly include the following: 

Why do websites need an anti-crawl mechanism? There are two reasons, one is to protect website security and reduce server pressure, and the other is to protect website data security. 

Crawler technicians and anti-crawler technicians have always been like left and right hands. If you have an anti-crawl mechanism, I will have anti-crawl technology, which can be crawled immediately. 

![avatar]( 2021062519051936.jpg) 

Today, we will introduce the anti-crawling mechanism and practical countermeasures of the website in detail. Generally, websites are anti-crawling from three aspects: 

1. User request headers 2. User behavior 3. Website directory and data loading method 

The first two are easier to encounter, and most websites are anti-crawling from these angles. The third type is used by some websites that apply Ajax, which increases the difficulty of crawling (to prevent static crawlers from using Ajax technology to dynamically load pages). 

This is the most common anti-crawler mechanism. When visiting certain websites, websites usually use a header file to identify whether the visit is a crawler, as a strategy for anti-crawler. 

Then we need to disguise headers. Many websites will detect the User-Agent of Headers, and some websites will detect Referers (the anti-theft chain of some resource websites is to detect Referers). 

If you encounter such anti-crawling mechanisms, you can directly add headers to the crawler, copy the browser's User-Agent into the crawler's headers, or modify the Referer value to the target website domain name. 

It is often overlooked. Through the packet capture analysis of the request, the referer is determined, and the access request header is simulated in the program. 

For anti-crawlers that detect headers, modifying or adding headers to the crawler can be easily bypassed. 

For example, open the Sohu homepage, first take a look at the header information of the Chrome (F12 opens the developer mode) as follows: 

![avatar]( eb1d2158cf78fb1c6c6adce238ed956e.png) 

As shown in the figure, the access header information shows the browser and system information (headers contain a lot of information, among which User-Agent is an identifier of the user's browser identity, which can be queried by yourself). 

The request module in urllib in Python provides the function of simulating browser access. The code is as follows: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957457742
 ```  
Access can be requested by add_header (key, value) or directly with the URL as a parameter 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957457742
 ```  
Where headers is a dictionary, in this way the crawler can be simulated as a browser to access the website. 

![avatar]( 20210625190707802.jpg) 

>  I have a lot of technical dry goods in my private stash, and fans can use them for free (click here). 

There are also some websites that detect user behavior, such as multiple visits to the same page by the same IP in a short period of time, or the same account performing the same operation multiple times in a short period of time. 

This kind of anti-creep requires enough IP to deal with it. 

(1) Most websites are in the former case. In this case, it can be solved by using an IP proxy. You can write a crawler specifically, crawl the public proxy IPs on the Internet, and save them all after detection. With a large number of proxy IPs, you can change an IP every few times a request, which is easy to do in requests or urllib, so that you can easily bypass the first anti-crawler. 

Write a crawler proxy: 

Steps: 

1. The parameter is a dictionary {'type': 'proxy ip: port number'} proxy_support = urllib.request. ProxyHandler ({}) 2. Customize, create an opener opener = urllib.request. build_opener (proxy_support) 3. Install opener urllib.request. install_opener (opener) 4. Call opener opener.open (url) 

Use a large number of proxies to randomly request target websites and deal with anti-crawlers 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957457742
 ```  
(2) For the second case, the next request can be made at random intervals of a few seconds after each request. Some websites with logical vulnerabilities can bypass the restriction that the same account cannot make the same request multiple times in a short period of time by requesting several times, logging out, logging in again, and continuing the request. 

Anti-crawl restrictions on accounts are generally difficult to deal with, and random requests for a few seconds may often be blocked. If you can have multiple accounts, switching to use is more effective. 

![avatar]( 20210625191729446.jpg) 

Most of the above situations appear on static pages, and there are some websites where the data we need to crawl is obtained through Ajax requests or generated through Java. 

Solution: Selenium + PhantomJS 

Selenium: Automated web testing solution that fully simulates the real browser environment and essentially all user actions 

PhantomJS: A browser without a graphical interface 

For example, obtain Taobao's personal details address: 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957457742
 ```  
Finally, let me summarize the anti-climbing mechanism and coping strategies mentioned earlier: 

Finally, let me tell everyone that the reptile world is indeed very interesting. Technology is innocent, and learning is OK, but the actual operation is enough, and do not touch the boundaries of the law. 

Thank you for reading and liking. I have collected a lot of technical dry goods that can be shared with friends who like my articles. If you are willing to take the time to study, they will definitely help you. The dry goods include: 

![avatar]( 17baf34c84e4483f9f9b3d9bb3341c44.png) 

![avatar]( 521e60d8459b40f2bd654b1a410926db.png) 

 Click on the business card at the end of the article to take it away.  

