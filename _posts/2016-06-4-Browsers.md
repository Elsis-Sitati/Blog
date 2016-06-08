---
layout: post
title: How Browsers/Internet Work 
---

The internet is a web of connected networks.At the most basic level,think of internet as your browser connecting to a server.
The browser makes a request to the server and the server sends a response to the browser.The server is just another machine 
connected to the internet.When you type the name of a website say elsissitati.com,your Internet Service Provider charter does
a Domain Name Service look up and translates elsissitati.com to an IP address.Any machine computer connected to the internet
has an IP address.The DNS basically says "hey elsissitati.com ,what IP adress have you been configured to?"It finds the server
that has been configured to that address and the browser sends you there.When you connect to the server it gives back a 
response.The response is usually the file and the content type.The browser knows how to treat what response its being given
by its content type.For example the index.html file will be loaded and the browser starts reading the file from top to 
bottom.It pauses when it finds a request for an asset.An asset is another file that needs to be requested e.g css and js.
A request usually contains two things,a header and a body.While a header is mandatory,it may or may not contain a post body.
Post body is used when sending data.Responses also have headers and a post body.
