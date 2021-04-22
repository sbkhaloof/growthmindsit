# The Coder's Computer
## choosing a text editor 
#### what is the text editor ?
###### it is a computer program used to write and manage your text . you can download , install or access it onloine using your browser .
###### and  the most important feature it should have :
+ code completion.
+ syntaxhighlighting .
+ a nice variety of themes(to  reduceeye strain and fatigue ).
+ he ability to choose from a healthy selection of extensions available when you need them.
#### some of text editor can all be downloaded and installed to your computer from the irrespective websites.
![](https://i.pcmag.com/imagery/articles/01rBnPopClrTbcmGbFMDwIE-1.1597666892.fit_lim.jpg)
![](https://e7.pngegg.com/pngimages/754/763/png-clipart-textwrangler-macos-text-editor-bbedit-cb-text-app-store-unix.png)
![](https://res.cloudinary.com/practicaldev/image/fetch/s--9F8ygOQO--/c_imagga_scale,f_auto,fl_progressive,h_720,q_auto,w_1280/https://dev-to-uploads.s3.amazonaws.com/i/ikysur95osy0deokuuji.png)
## Linux Tutorial - 1. The Command Line
#### A command line, or terminal, is a text based interface to the system. You are  enter commands and feedback will be given to you similarly as text. The command line typically presents you with a prompt. As you type, it will be displayed after the prompt. 
##  few places to start looking _ opening a terminal
+ If you're on a Mac then you'll find the program Terminal under Applications -> Utilities. An easy way to get to it is the key combination 'command + space' which will bring up Spotlight, then start typing Terminal and it will soon show up.
+ If on Linux then you will probably find it in Applications -> System or Applications -> Utilities. Alternatively you may be able to 'right-click' on the desktop and there may be an option 'Open in terminal'
+  you are on Windows and intend to remotely log into another machine then you will need an SSH client. A rather good one is Putty .
## Linux Tutorial - 2. Navigation
#### the first command we are going to learn is pwd which stands for Print Working Directory. so pwd tell as where are we.
#### the command which answer what is current location  is ls. It's short for list. Let's give it a go.
#### Absolute and Relative Paths:
###### Absolute paths specify a location (file or directory) in relation to the root directory. You can identify them easily as they always begin with a forward slash ( / ) but Relative paths specify a location (file or directory) in relation to where we currently are in the system. They will not begin with a slash.
###### Here are some more building blocks you may use to help build your paths:
+ ~ (tilde) 
+ . (dot) 
+ ..(dotdot)
#### command called cd which stands for change directory used to moved around a bit 
## Linux Tutorial - 3. More About Files
#### with linux everything is file  A text file is a file, a directory is a file, your keyboard is a file (one that the system reads from only), your monitor is a file (one that the system writes to only) etc. so you should keep in mind the behaviour of Linux as you manage files and directories. 
+ linux is an extensionsless system 
###### A file extension is normally a set of 2 - 4 characters after a full stop at the end of a file, which denotes what type of file it is. some of extensions are file.exe ,file.txt ,file.png.
###### nder Linux the system actually ignores the extension and looks inside the file to determine what type of file it is. 
+ linux is case sensetive 
+ space in name 
+ hidden file and directories .
###### If the file or directory's name begins with a . (full stop) then it is considered to be hidden.  The command ls which we have seen in the previous section will not list hidden files and directories by default. We may modify it by including the command line option -a so that it does show hidden files and directories.
