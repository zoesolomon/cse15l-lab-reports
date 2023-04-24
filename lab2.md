## Lab2: Servers and Bugs

This report shows examples of a server and its commands, as well as bug fixes.

## PART 1: Building a Server

Server called "String Server" that displays the query input into the math url.

![Image](handler.png)
![Image](server.png)

In the first screenshot below, the method being called is the main method in the StringServer class, as that starts the server, while in the other screenshots it is the handleRequest method in the Handler class being called. 

The input to start the server (in the main method) is the port number, which is taken as a list parameter and saved as a field called "port" when the method instantiates a new handler. The parameters in the Handler class come from the url put into the local host. The two relevant fields in this method are the list parameter[1], which is split at the equals sign in the path, and stored the text to be added, and the String s which is concatenated with the new paramter[1] everytime there is a new inpput in the url. These values due change with specific requests, as it depends on the user input.

![Image](start.png)

![Image](serverhome.png)

![Image](hi.png)

![Image](hello.png)

![Image](how.png)

## PART 2: Debugging



## PART 3: Discovery

Something that I learned in this week that I hadn't known previously was how to create a server, as I didn't even know anything like this was possible without a lot more coding.





