---
layout: post
title: How Browsers Work 
---

The internet is a web of connected networks.At the most basic level,think of internet as your browser connecting to a server.
The browser makes a request to the server and the server sends a response to the browser.The server is just another machine 
connected to the internet.When you type the name of a website say elsissitati.com,your Internet Service Provider charter does
a Domain Name Service look up and translates elsissitati.com to an IP address.Any machine computer connected to the internet
has an IP address.

The DNS basically says "hey elsissitati.com ,what IP adress have you been configured to?"It finds the server that has been configured to that address and the browser sends you there.When you connect to the server it gives back a response.The response is usually the file and the content type.The browser knows how to treat what response its being given
by its content type.For example the index.html file will be loaded and the browser starts reading the file from top to 
bottom.It pauses when it finds a request for an asset.An asset is another file that needs to be requested e.g css and js.

A request usually contains two things,a header and a body.While a header is mandatory,it may or may not contain a post body.
Post body is used when sending data.Responses also have headers and a post body.
When a person for example types elsissitati.com,a request is made to the server.the server sends back an index.html file
as a response.The browser starts loading the file from the top.Depending with where you have referenced your css,if it finds
the css reference in the <head> tag it is going to pause and make a request for the css file from the server.The server will 
send a response containing the css file.The browser will then check how to display the html elements as defined by the css.
It is good practise to put the css in the <head> tag to avoid a flash of unstyled content.This when a webpage loads and it is
ugly at first and then it flickers into being beautiful.This is because your browser is first loading the elements in your <body>
tag and then loading the css to dictate how to display these elements later.It is best practise to put your scripts 
before the closing </body> tag.This is to facilitate the browser to first load the page and then later load the scripts and 
activate the script functionalities.This helps improve faster load times.Minifying the css and js also improves the load 
time.
