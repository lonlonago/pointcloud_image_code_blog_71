NetEase Cloud Music has always been a great platform for listening to music, especially the recommendation algorithm. I personally think it is more popular than a certain Q music. I have always used NetEase Cloud to listen to music. 

![avatar]( 20210626154515967.png) 

Today, I will teach you a way to crawl the comments of any song in the NetEase cloud and generate a special word map. Those who are interested in crawlers can try to practice their hands. After mastering the method, they can crawl any song they want. 

###  First, the effect 

Let's take a look at the effect of the final word picture effect, still "No Man's Island" as an example, although it is a song 3 years ago, but there are still many listeners like this song, so far there have been more than 250,000 comments. 

![avatar]( 20210626154748480.png) 

Let's take a look at what 250,000 people were saying while listening to this song, and see the renderings crawled out by the comments: 

![avatar]( 20210609140925390.jpg) 

###  Second, the technology used 

This technical difficulty is not large, mainly using selenium and several third-party libraries can be achieved, first give you a simple technical explanation. 

Selenium is a tool for web application testing. Selenium tests run directly in the browser, just like a real user, without being suspected by the website to be crawled. 

Automatically render all response content, which can directly bypass the operation of js encryption. As long as the data is displayed on the browser, it can be obtained by the headless browser, and it can be almost visible and crawled. 

Jieba library, wordcloud library, MySQLdb, numpy library. 

###  III. Source code analysis 

1. Crawl the comments into the library section. 

![avatar]( 20210609142819244.jpg) 

  2. Perform renderings display visualization. 

![avatar]( 20210609144113129.jpg) 

If you need the source code, you can leave a message "NetEase Cloud" in the comment area below, then chat with me privately, and I will send you the source code, or find my assistant in my technical exchange group. 

###  Fourth, crawl any song comments 

After mastering this method, we can not only climb "No Man's Island", but also climb other songs. The method is the same, and it can be completed through these few steps. 

First of all, there is a URL for the request URL in our code, which is the string of addresses in the address bar. It needs to be declared that it is only for the songs of the web version of the NetEase Cloud Music official website. The example picture is as follows: 

![avatar]( 20210609145023219.jpg) 

![avatar]( 20210609144953811.jpg) 

  If you still need visualization, just follow the above method. Thank you for reading and liking. I have collected a lot of technical dry goods, which can be shared with friends who like my articles. If you are willing to take the time to study, they will definitely help you. The dry goods include: 

![avatar]( 17baf34c84e4483f9f9b3d9bb3341c44.png) 

![avatar]( 521e60d8459b40f2bd654b1a410926db.png) 

 Click on the business card at the end of the article to take it away.  

