HowBrowsersWork



Hi I am Qusai

I will explain the functionalities  of the web browser , but before we start lets define a Web Browser...



A web browser is a software application used to access the Internet in order to retrieve/present/display information




Function of Browser:
The main function of a Browser is to present resources that have been requested by the user from the server, and display it in the browser window. Usually this resources are an HTML ,XHML ,PDF ,  images, video or any other content . The location of the resources is determined by the user input in the address bar it's called URL(Uniform Resource Identifier ). you can think of it as the index that refer to that specific content in the server DB (data base).




The way Browser interpret   HTML files is specified buy the HTML & CSS specifications .The HTML & CSS specifications are set by W3C organization(World Wide Web Consortium) , its standard organization for Web. for years Browsers confirmed only part of the specifications and developed their own extensions . That caused a serious compatibility issues for Web authors and developers.
Now days most of the Browsers more or less confirm to the specifications .




Browser User Interface or (BUI):
is a method of interacting with an application , typically hosted on a remote device, through controls presented in the web browsers.





Browser User Interface has a lot in common with each other.
The W3C dose not include a UI in the Web specifications , even though different Browsers share the same concept of presentation when it comes the  Browser UI

Common UI elements:
-Address bar for entering URL
-Home Button
-Back/Forward buttons
-Refresh Button
-Bookmark options

The reason why Browsers UI has lot of similarities  is mostly because developer imitating each other , and years of practice that shaped the UI form that could best fit a Web browsers .




Browsers Hight level structure

1. The user interface  :
this include everything browser display except the window where you see the requested web page .

2. the browser engine : marshals actions between the UI and the rendering engine

3.The rendering engine :
 responsible for displaying the requested content .
Eg. if the requested content is HTML the rendering engine parse HTML&CSS and display the parsed content on the screen.

4. Networking : for network calls such as HTTP (Hyper Text Transfer Protocol) requests, using different implementations of different platform behind a platform-independent   


UI backend :used for drawing basic widget like combo boxes and windows .
This backend exposes a generic interface that is not platform specific, underneath it uses the o/p system user interface method .


5. Javascript interpreter: it is used to parse and  execute javascript codes.



6. data storage :
This is a persistence layer. The browser may need to save all sorts of data locally, such as cookies. Browsers also support storage mechanisms such as localStorage, IndexedDB, WebSQL and FileSystem.
