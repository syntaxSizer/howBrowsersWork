#HowBrowsersWork



Hi I am Qusai

I will explain the functionalities of web browser , but before we start lets define a Web Browser...



A web browser is a software application used to access the Internet in order to retrieve/present/display information




####Function of Browser:
The main function of a Browser is to present resources that have been requested by the user from the server, and display it in the browser window. Usually this resources are an HTML ,XHML ,PDF ,  images, video or any other content . The location of the resources is determined by the user input in the address bar it's called URL(Uniform Resource Identifier ). you can think of it as the index that refer to that specific content in the server DB (data base).




The way Browser interpret   HTML files is specified buy the HTML & CSS specifications .The HTML & CSS specifications are set by W3C organization(World Wide Web Consortium) , its standard organization for Web. for years Browsers confirmed only part of the specifications and developed their own extensions . That caused a serious compatibility issues for Web authors and developers.
Now days most of the Browsers more or less confirm to the specifications .




####Browser User Interface or (BUI):
is a method of interacting with an application , typically hosted on a remote device, through controls presented in the web browsers.
https://en.wikipedia.org/wiki/Browser_user_interface





####Browser User Interface has a lot in common with each other.
The W3C dose not include a UI in the Web specifications , even though different Browsers share the same concept of presentation when it comes to Browser UI

#####Common UI elements:
-Address bar for entering URL
-Home Button
-Back/Forward buttons
-Refresh Button
-Bookmark options

The reason why Browsers UI has lot of similarities  is mostly because developer imitating each other , and years of practice that shaped the UI form that could best fit a Web browsers .





#####Browsers Hight level structure

1.The user interface  :
  this include everything browser display except the window where you see the requested web page .


2.the browser engine :
  marshals actions between the UI and the rendering engine

3.The rendering engine :
  responsible for displaying the requested content .
  Eg. if the requested content is HTML the rendering engine parse HTML&CSS and display the parsed content on the screen.
  rendering engine by default parse HTML&CSS documents , but it can parse other document via plug-in

  http://www.html5rocks.com/en/tutorials/internals/howbrowserswork/#The_rendering_engine


4.Networking : for network calls such as HTTP (Hyper Text Transfer Protocol) requests, using different implementations of     different
  platform behind a platform-independent



5.UI backend :used for drawing basic widget like combo boxes and windows .
  This backend exposes a generic interface that is not platform specific, underneath it uses the o/p system user interface method .



6.Javascript interpreter: it is used to parse and  execute javascript codes.




7.data storage :
  This is a persistence layer. The browser may need to save all sorts of data locally, such as cookies. Browsers also support storage mechanisms such as localStorage, IndexedDB, WebSQL and FileSystem.



 The main flow:

 the rendering engine will start getting the content of the requested document from the network layer.This usually will be done in 8kB chunks.

 parsing HTML to construct the DOM tree ----->  render tree construction ----->  Layout of the rendering tree


http://www.html5rocks.com/en/tutorials/internals/howbrowserswork/#The_main_flow

DOM (Document Object Model).
http://www.html5rocks.com/en/tutorials/internals/howbrowserswork/#DOM


render tree
http://www.html5rocks.com/en/tutorials/internals/howbrowserswork/#Render_tree_construction


HTML parser:
the job of HTML parser is to parse the HTML markup into parse tree

http://www.html5rocks.com/en/tutorials/internals/howbrowserswork/#HTML_Parser

The HTML grammar definition:
the vocabulary and syntax of HTML are define in W3C specifications that i mentioned at the beginning
here:http://www.html5rocks.com/en/tutorials/internals/howbrowserswork/#w3c


Not a context free grammar

As we have seen in the parsing introduction, grammar syntax can be defined formally using formats like BNF.

Unfortunately all the conventional parser topics do not apply to HTML (I didn't bring them up just for fun–they will be used in parsing CSS and JavaScript). HTML cannot easily be defined by a context free grammar that parsers need.

There is a formal format for defining HTML–DTD (Document Type Definition)–but it is not a context free grammar.

This appears strange at first sight; HTML is rather close to XML. There are lots of available XML parsers. There is an XML variation of HTML–XHTML–so what's the big difference?

The difference is that the HTML approach is more "forgiving": it lets you omit certain tags (which are then added implicitly), or sometimes omit start or end tags, and so on. On the whole it's a "soft" syntax, as opposed to XML's stiff and demanding syntax.

This seemingly small detail makes a world of a difference. On one hand this is the main reason why HTML is so popular: it forgives your mistakes and makes life easy for the web author. On the other hand, it makes it difficult to write a formal grammar. So to summarize, HTML cannot be parsed easily by conventional parsers, since its grammar is not context free. HTML cannot be parsed by XML parsers.

(Backus-Naur Form) BNF:https://en.wikipedia.org/wiki/Backus%E2%80%93Naur_Form



CSS parsing:
Remember the parsing concepts in the introduction? Well, unlike HTML, CSS is a context free grammar and can be parsed using the types of parsers described in the introduction.In fact the CSS specifications define CSS lexical and syntax https://www.w3.org/TR/CSS2/grammar.html



you can find out more about web browsers in this link :http://www.html5rocks.com/en/
there is steel many mechanism that contribute to the Browser in order to function the way it dose.
