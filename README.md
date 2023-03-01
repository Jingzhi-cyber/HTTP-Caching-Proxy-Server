This project is an http proxy – a server whose job it's to	forward	requests to the origin server on behalf	of the client.

It supports HTTP GET, POST, and	CONNECT methods. 

It will also cache responses, and when appropriate, respond with the cached copy of a resource rather than re-fetching it.

This project used boost library to parse the http request and response. If you want to compile our source code and run, you need to do 

`sudo apt-get install libboost-all-dev`

to install the boost library first.

To run this proxy within docker, you can run

`sudo docker-compose up`

Now you need to change the proxy of your web browser to this proxy with port 12345. After that you can open web pages with this proxy.

The testcases we used is in testcases.txt and danger_log.txt contains information about possible dangers in our program.
