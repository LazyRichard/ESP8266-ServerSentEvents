# Server-Sent Events / EventSource Demo

This demonstrates how to use EventSource with PHP or ESP8266 Event Generators.

Here's a small explanation and a video demo of the scripts:  
https://www.claudiuscoenen.de/2015/09/generating-server-sent-events-on-arduino/


## ESP8266

Use a bare metal ESP8266 board, add Something to pins 5, 6 or A0. 
Enter a free IP in the `.ino` file on which your ESP8266 will be available.
You can use this technique for update only some parts of your webpage instead
of refresh the whole page, really useful in IoT programming.

Alter the IP in `index.html` to match your ESP8266's IP and choose to use in
a server.on() handler or just in the root page resource.


## PHP

Change the script in `index.html` to point to `source.php` - the code is already
there, you just need to remove a comment.

Run `php -S 0.0.0.0:8000` in this directory, this will create a simple webserver.


## EventSource Resources

* [W3C Specification](http://www.w3.org/TR/eventsource/)
* [Can I Use](http://caniuse.com/#feat=eventsource) hint: in 2015, everything but IE/Edge is fair game.
* [HTML5Rocks Tutorial](www.html5rocks.com/en/tutorials/eventsource/basics/)
