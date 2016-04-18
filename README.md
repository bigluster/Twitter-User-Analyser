# Twitter-User-Analyser

// Twitter account detail

/* Version 1.0
A Qlik Sense app that is using Qlik REST Connector to load data from Twitter. Is has some limitation of rows loaded from Twitter.


To use this app in Qlik Sense you need to: 

Download


1. Download Qlik REST API Connector http://market.qlik.com/rest-connector.html


2. Download extension WordCloud https://github.com/cleveranjos/br.com.clever.wordcloud/ or https://community.qlik.com/docs/DOC-7794



Twitter


1. Have or Create an Account on Twitter (for authentication)


Apigee


1. Go to https://apigee.com/console/twitter


2. Choose service https://api.twitter.com/1.1


3. Choose authentication OAuth 1 and give access/autorize app to your twitter account


4. In left menu "Select an API method" select Timelines - user_timeline 


5. Then in Query fill in the User ID - you can find User ID on http://gettwitterid.com/ by typing twitter username (screen name)


6. Fill in screen_name (username for twitter)


7. Fill in Since ID - the max date from which will be loaded data in some interval to history


8. Click on send button


9. The data for REST connector will appear in the Request URL and on the left side in Request


10. Dont close the website, you will need it for next steps.


Now you have all information needed for Qlik Rest Connector, to create new Qlik Sense connection you need to:

![Screen 2](https://raw.githubusercontent.com/marosvongrej/Twitter-User-Analyser/master/QSSET1.png "Screen 2")

![Screen 2](https://raw.githubusercontent.com/marosvongrej/Twitter-User-Analyser/master/QSSET2.png "Screen 2")

1. Open data load editor and in the right corner click create new connection


2. Choose Qlik REST Connector and name the connection to Twitter


3. URL - copy the "Request URL" from Apigee website 


4. Timeout - 30


5. Check autodetect response type and Key generation stragegy - Sequence ID


6. Windows anthentication - NO


7. Your twitter mail and password


8. Use certificatie - NO


9. Pagination type - NO


10. In query headers create 3 rows:
    a. Authorization
    b. Host
    c. X-Target-URI


11. Copy the information from Apigee (you can find it by clicking on Send button in apigee and after the server response, 
	they will appear on the left side in Request.


12. Test conection    


13. In the sheet Twitter_user you have load script


14. Now you can Load data or preview the data.


15. ThatB4s all!

Enyoj!

Maros twitter: @MarosVongrej Linkedin: Maroš Vongrej https://cz.linkedin.com/in/maroš-vongrej-927a7153
    
*/
