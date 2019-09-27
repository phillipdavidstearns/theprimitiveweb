# Primitive Web (1.0) Publishing

## Hello!

![](resources/images/hello.gif)

* **`whoami`** - Phillip David Stearns (Artist, Designer, Engineer, Educator)
* **what is this?** - A walkthrough to re-discover the Internet and learn how to use the command line to make things.
* **who is it for?** - Sadly, only folks with Mac OSX, Linux, or Unix operating systems.
* **why?** - The Internet is a place for everyone and anyone can make a website. Internet tools can be used to locally host info offline (Intranet).


## 1. press `command+spacebar` to bring up the spotlight search bar

![](resources/images/CommandSpacebar.png)

## 2. type `terminal` and press enter to launch the terminal

![](resources/images/spotlight.png)

### This is your terminal

* We're used to the **graphic user interface (GUI)**
* terminal.app gives you a **command line interface*(CLI)**.
* **how to use**: type a command and then press enter

![](resources/images/terminal.png)


## 3. run `pwd` to see what your preset working directory is

You should get something like:

```
/Users/coursework
```

* `pwd` shows us the **p**resent **w**orking **d**irectory

## 4. run `ls` to see what it in that directory

![](resources/images/ls.png)

* **`ls`** "list directory contents"
* find out more using the `man` or "manual" command: `man ls`
* exit from the manual by pressing `q`

## 5. run `ls -ahl` to get more details about the directory contents

![](resources/images/lsahl.png)

`-ahl` is an argument passed to the `ls` command. This argument contains the options:

* `-a` - list **a**ll of the contents (even hidden files)
* `-h` - show size in a **h**
* `-l` - output in a sigle-column **l**ist

## 6. run `cd Documents` to change your present working directory

**`cd`** changes your working directory

## 7. run `la -ahl` to view its contents

![](resources/images/documents.png)

## 8. run `mkdir mywebpage` to create a directory for your webpage


## 9. run `cd mywebpage` to change to that directory

## 10. run `pwd` to confirm your path


## 11. run `ls` to confirm it's empty


## 12. run `echo 'Hello World!' > index.html` to create a webpage

## 13. run `python -m SimpleHTTPServer 8080`

This will launch a server hosting your webpage on your own computer at `localhost` or `127.0.0.1`

* Python is a programming language.
* The `python` command, when entered by itself, is used to start the python language interpreter.
* `-m` tells python to execute a built-in module, in this case `SimpleHTTPServer`
* `SimpleHTTPServer` takes a port number as an argument, in this case we specify `8080` but it could be anything between `2` and `65535`

##14. open a web browser and enter `localhost:8080` in the URL navigation bar

![](resources/images/localhost.png)

## 15. return to the terminal and press `command+t` to create a new tab

* We need to leave the terminal window in which we ran the `SimpleHTTPServer` open and running.

## 16. run `pwd` to check that you're in the directory of your website

## 17. run `mkdir images; cd images` to create a directory called "images" and change to it

Using

## 18. grab a random cat or dog gif from the web:

* for cat poeple, run: `wget 'https://thecatapi.com/api/images/get?format=src&type=gif' -O cat.gif`
* for dog people, run `wget 'https://api.thedogapi.com/api/images/get?format=src&type=gif' -O dog.gif`

## 19. run `ls -alh` to confirm that it shows up as `./images/cat.gif` or `./images/dog.gif`

## 20. run `nano ../index.html` and edit the webpage to read:

For cats:

```
<html>
	<div align=center>
		<img src="images/cat.gif"><br>
		Meowwo World!
	</div>
</html>
```

For dogs:

```
<html>
	<div align=center>
		<img src="images/dog.gif"><br>
		Bowwow World!
	</div>
</html>
```

## 21. press `control+o` and then `enter` to save

![](resources/images/)

## 22. in your browser, click refresh

![](resources/images/)

## BONUS!



## Clean up!

1. Turn off the `SimpleHTTPServer` by either closing the tab or by activating the terminal tab and pressing `control+c`
2. Delete files in the **images** directory using `rm ~/Documents/mywebpage/images/*`
3. Delete the **images** directory using `rmdir ~/Documents/mywebpage/images`
4. Delete files in the **mywebpage** directory using `rm ~/Documents/mywebpage/*`
5. Delete the **mywebpage** directory using `rmdir ~/Documents/mywebpage`

All done!