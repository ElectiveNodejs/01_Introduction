# #1 Tutorial: My first Webserver
In this forst tutorial you are going to create a webserver with a webpage and deploy it to an online host. So the result will be your first, public accessable Node.js website.

You will be guided through installing Node.js on your computer, creating a webserver on your Node.js installation. This webserver will be accessable to anyone on the local network you are currently on. Then you will create an account at Heroku, a host, where you will be deploying your new website. At the end you will be deploying the website to Azure and you will have your first Node.js public accesable website up and running.

## Installing Node.js

First of all you need to download and install Node.js. The Installations is pretty straight forward, but if you need it,  guides kan be found here:

* [Installing Node.js on a Mac](https://www.lynda.com/MyPlaylist/Watch/5464398/110731?autoplay=true)
* [Installing Node.js on Windows](https://www.lynda.com/MyPlaylist/Watch/5464398/110731?autoplay=true)
* [Installing Node.js on Linux](https://www.lynda.com/MyPlaylist/Watch/5464398/110731?autoplay=true)

To test if your installation went ok, and that you have Node.js on your computer, open the console and type:

<pre>node --version</pre>
Then you should see something like this:

<pre>node --version
v4.4.7</pre>

The version number could differ in your case. If you do not see this, something went wrong in the installation process, and try to install Node.js again.

## Create a local Webserver

Now let´s create our first server. Create a folder and in it a file called server.js, containing the following code.

```prettyprint javascript
    var http = require('http');

    var server = http.createServer(function (req, res) {
      res.writeHead(200, {'Content-Type': 'text/plain'});
      res.end('Hello World\n');
    });

    server.listen(3000);

```

Start the server from the console by browsing to the folder you just created and type:

```javascript   
   node server.js   
```

Now open your browser and type in the url: http://localhost:3000/

![](/tutorials/img/browser.png)

If what you made now is indeed a webserver, and not just a document saying “Hello World”,  you should be able to access this site from you phone or another computer.

Get the ip-address of you machine (the server) and then make sure that your phone is on the same network as your computer (the server). Type in 10.108.10.86:3000 (this is my ip, you should of cause use yours).

<img src="/tutorials/img/iphone.png" width="400" >


Hopefully you see this, otherwise: “are your devices on the same network” ?

## HTML 

If we go one step further we can show a html page instead of the simple text page above.    

TODO: write tutorial    

## JSON

The aproach we will take in this elective is to create an API.

TOdo: write tutorial


## Deploy to an online host

TODO: write tutorial


## Create a simple frontend JQuery app

TODO: write tutorial


 ___ 
<footer align="right" style="font-size: small">(heavily inspired by http://howtonode.org/deploy-blog-to-heroku)</footer>
