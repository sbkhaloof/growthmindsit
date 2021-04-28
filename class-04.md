# HTML Links, JS Functions, and Intro to CSS Layout
## links :are the defining feature of the web because they allow you to move from one web page to another .
### we can writting a link using <a> as you can see in figure :
![](https://www.computerhope.com/jargon/h/html-tag.gif)
### Users can click on anything that appears between the opening <a> tag and the closing </a> tag and will be taken to the page specified in the href attribute. When you link to a different website, the value of the href attribute will be the full web address for the site, which is known as an absolute URL. Browsers show links in blue with an underline by default.
### you can use links to :
+ Linking to other sites (use absolute URL).
+ Linking to other PAges on the sAme site (use relative URL).
+ email link :  this time the value of the href attribute starts with mailto: and is followed by the email address you want the email to be sent to. On the right you can see that an email link looks just like any
other link but, when it is clicked on, the user's email program will open a new email message and address it to the  person specified in the link.
#### oPening Links in A neW WinDoW .If you want a link to open in a new window, you can use the target attribute on the opening <a> tag. The value of this attribute should be _blank .
## <a chrf -"url"target-"blank">
+ Linking to A sPeciFic PArt oF the sAme PAge : you need to identify the points in the page that the link will go to. You do this using the id attribute The value of the id attribute should start with a letter or an underscore (not a number or any other character) and, on a single page, no two id attributes should have the same value.To link to an element that uses an id attribute you use the <a> element again, but the value of
the href attribute starts with the # symbol, followed by the value of the id attribute of the element you want to link to.
+ Linking to A sPeciFic PArt oF Another PAge: the href attribute will contain the address for the page (either an absolute URL or a relative URL), followed by the # symbol, followed by the value of the id attribute that is used on the element you are linking to.
## layout 
### Key ConCepts in positioning eLements
#### buliding blocks : CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box. so you should know Block-level elements start on a new line sach as : <h1> <p> <ul> <li> . but inline elements flow in Between surrounding text as <img> <b> <i> .
#### ControLLing the position of eLements as( normal flow ,relative Positioning , aBsolute Positioning ,fixed Positioning ,floating elements) .
## “Functions, Methods, and Objects
### Browsers require very detailed instructions about what we want them to do. Therefore, complex scripts can run to hundreds (even thousands) of lines. Programmers use functions, methods, and objects to organize their code.
### Functions let you group a se ries of statements together to perform a specific task. If different pa rts of a script repeat the same task, you can reuse the function (rather than repeating the same se t of statements).
### declearing the function :
![](https://raddevon.com/wp-content/uploads/2019/07/function-declaration-diagram-1024x282.png)
### after you decleae the function you need to execute all statment inside it with just one line this is called callin function 
## addExcitement(x);
### also you can get value(s) out of a function this is by using return keyword and the value(s) which you need it at the end of the function 
## 6 Reasons for Pair Programming
### While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard.The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs.
### Pair programming touches on all four skills: developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves.
### tere are alot of benefits for Pair Programming:
+ Greater efficiency
+ Engaged collaboration
+ Learning from fellow students
+ Social skills
+ Job interview readiness
+ Work environment readiness