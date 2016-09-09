# ContentManagement

React App for Content Management

###WHAT IT NEEDS TO RUN

* APACHE
* PHP
* MYSQL
* NPM (Node)

You need to/can download WAMP OR XAMP according to your choice. Please install node. My version of node 4.4.7.

For WAMPSERVER 2.5
****
1. You can find the WAMP server download link here -> http://www.wampserver.com/en/ 
2. Either extract the code ZIP or git clone in any path you want.

HTTPD.CONF CHANGES
****

* You can find httpd.conf in the folder where apache is installed. In my case it is "C:\wamp\bin\apache\apache2.4.9\conf\" as my wamp is installed in C: Drive.
* Find all "/var/www" in httpd.conf in WAMP and point it to the path wherever this project exists. 
* Uncomment LoadModule rewrite_module modules/mod_rewrite.so in httpd.conf to enable Rewrite engine in .htaccess


###CODEIGNITER CONFIG

1. .htaccess -> Changed to remove index.php from the URL

###IMPLEMENTATION

There is one main URL

1. http://localhost (Your base URL can be different)-> The main content Managemet App functionality can be obtained here.


###STEPS

1. Go to the above said URL and look into the specifications as asked.
2. Please go to folder js/customContent and run npm install

###CODE STRUCTURE

BACKEND - CODEIGNITER 2.2.6

FRONTEND- REACTJS
****

1. All js files can be obtained under /js/customContent folder
2. src/components, src/reducers, src/actions are all the necessary folders for react redux.
3. JSON file can be found in src/json
4. Build happens in public/build -> bundle.js

CSS and FONTS
****

1. All custom css files , google fonts and images are found under /css , /fonts , /img respectively.

###FUNCTIONALITY

1. The Content Management app is responsive. Checked using Google Chrome Emulator.
2. Hovering on the images causes to show three links Open, Delete and Print with an Overlay
3. Headers and paragraph are one block and kept fixed even if the contents are scrolled.
4. Minimum use of colors are used to follow the CSS norms.
5. Icon is a sprite image from Pinterest.
6. Each Image has a text which can be changed from JSON file. JSON file is present in the folder mentioned above.
7. Open causes React Modal to open, Delete hides the respective image and Print opens a new Window with a Print Console as done in Google Maps.
8. Ellipsis are not used. But there is a Style Class in CSS which can be used if required.
9. Neat Padding and Margins are used.
