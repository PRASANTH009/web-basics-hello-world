# web-basics-hello-world
A super-basic (and ugly!) web page to show off the basics for SoT hackfest (html, css, js...).

Following this readme should help to prepare you for a weekend of API hacking by familiarising you with the basics of git, running a simple python server, and playing around with some web technologies to get a basic webpage to display some data from a simple API.

## Fork the repo and setup git
Login to Github if you haven't already (create an account if you need to).

Up the top right of this page you will see a button labelled **Fork**. Clicking this will make a 'copy' of this repo (repository) for you. This copy will be yours to play with as you wish. You can make commits and branches as much as you want to without affecting the original repo. So do that and then continue on with this readme (which will be available in your forked copy).

So now that you have your very own copy of my repo we need to get the code onto your machine. If you are familiar with git you can clone it down however you wish.

If you are not familiar with git I recommend [getting GitHub Desktop from here](https://desktop.github.com/). Its fairly easy to use and is a good option for Windows and Mac users. (At some point though you should absolutely invest some time in learning how to use git via command line/terminal). Find the option to clone a repository in GitHub Desktop. It will ask for a url. On the GitHub page for your forked repo click the **Clone or download** button. Copy the URL from there into the URL field in GitHub Desktop and then clone the repo to your machine.

Wooo! If everything went smoothly you should now have a copy of the code on your machine.

## Viewing the webpage in your browser
I recommend using the simple python server to serve up the webpage locally (You will need python installed https://www.python.org/ (If you have a Mac or a Linux machine you probably already have it installed)).

We need to use the command line to run the python server. [Mac users can use Terminal](http://www.wikihow.com/Open-a-Terminal-Window-in-Mac), [Windows users can use the Command Prompt](http://www.digitalcitizen.life/7-ways-launch-command-prompt-windows-7-windows-8), and Linux users should use whatever terminal app comes with their distro.

In your terminal/command line app navigate to the folder where index.html is located in your cloned repo (If you don't know what to do [Windows users can look here](http://www.digitalcitizen.life/command-prompt-how-use-basic-commands), [Linux and Mac users can look here](http://linuxcommand.org/lc3_lts0020.php)). Then run the command `python -m SimpleHTTPServer 8000`. When that is running you can point your browser to http://localhost:8000 to see the page running.

_Note: SimpleHTTPServer will default to serving the index.html file at the root url_

_Note: If you are using python 3 then I think you will need to run_ `python3 -m http.server 8000` _instead._

_Note: You might be able to just open the index.html page in a browser, but most browsers have security features that disable a bunch of things we might need when loading files locally. The python server will help us get around these security restrictions._

## Working with web stuff
The repo you forked and cloned contains a web page that is pretty useless. There are a bunch of things you can fix up to make it better, and in doing so get to play with most of the core things that make web pages work.

I recommend getting into the habit of working on one thing at a time and making a git commit for each thing you do. This way you have a history of changes that can help you if you (or someone else) makes a mistake and breaks something later (usually right before presentation time because life is like that haha).

To make a commit in GitHub desktop all you need to do is make some changes to the files in your local repo. The changes should appear in the GitHub Desktop app. Tick the files with changes that you want in the commit and enter the commit message details in the bottom right of the app. Click the commit button to make the commit! You can then sync the commits you have made on your local copy to your copy on github.com with the sync button up the top (which can also be used to pull down changes that have been made on the github.com copy if your local copy doesn't have them)

A good plain text editor to use for editing the files is Atom. [You can get it here](https://atom.io/).

_Note: Your browser will have a developer console you can use to debug things as you make edits. [Chrome users can look here](https://developer.chrome.com/devtools) and [Firefox users can look here](https://developer.mozilla.org/en-US/docs/Tools/Web_Console/Opening_the_Web_Console). For everyone else you will have to google around..._

Here are the things to fix up on the page:
* Make the heading say something useful by editing the h1 tag in index.html _(maybe something like 'hello world' yeah?)_
* Make the purple text purple by filling in the definition for the 'purple' css class in index.css _(If you want to learn more [here is a good guide for getting started with css](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS). I recommend looking at the [tutorial for css selectors](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Selectors) as it comes in handy for interacting with the page via javascript)_
* Make the button print some text into the results-area div by binding a javascript function to the click action on the button element _(hint: start with line 11 in index.js.)_
* Do something interesting with the fetchRandomWord function (which uses the http://www.setgetgo.com/randomword/ API) _(Maybe you can put the word it gets on the screen when the button is clicked?)_

Once you've done all this you can carry on and play with things as much as you like. Add a paragraph to the page describing your idea for the ultimate burger, or add some stock images of scientists doing science things. Or maybe you can make the page less ugly with some css styling or do something fancy with javascript like displaying the current system time? You can also use javascript to explore some data from some other APIs that are out there.

## Completed example
If you want to you can checkout the branch called `example` to see what I did to finish the page. It might also help you if you get a bit stuck.

In GitHub Desktop you can click the branch button at the top to switch branches
