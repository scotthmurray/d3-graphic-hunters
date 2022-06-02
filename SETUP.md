# SETUP

To work with D3, you need three things:

- a text/code **editor** (I recommend [Atom](https://atom.io))
- a current web **browser** (I recommend [Chrome](https://www.google.com/chrome/index.html))
- a local web **server**

I trust you to download and install the first two. 😁

Let’s talk about how to get a **local web server** up and running on your computer.  First, what does that even mean?

## What's a local web server?

Normally, web servers are “remote,” meaning they are running on other computers, somewhere “out there” and not here, right in front of you.  (Sometimes we call this “the cloud,” but, to be honest, the cloud is just other people’s computers.)

So, normally when you’re “surfing” the web (another misnomer!), your web **browser** is initiating requests for HTML pages and other resources from **remote** web servers.

When you’re **developing** your own web pages, it is much faster to work **locally**, meaning the web server is running on your own computer, right in front of you (i.e., not in the cloud).

So, in this case, you have *two* pieces of important software running on the same computer:

- the web browser
- the web server

When the browser requests a web page, it is requesting the page from the web server — the same as usual, only now the web server is running on the same computer.

This is great for web development, because you're editing, saving, serving, and viewing all your files from the same computer, so everything is super fast. No need to transfer files over a network — they’re all right there! 😎

## Setting up a local web server

The good news is there are lots of ways to set up and run your own web server locally.

The bad news is there are lots of ways to set up and run your own web server locally.

Let’s find the way that’s right for you.

### Python Web Server

If you’re on a Mac or Linux machine, you probably already have Python installed. If you’re using Windows and you know you have Python already, please follow along.

**If you are comfortable with the command-line,** this is the easiest way to get a web server up and running:

1. Open a new terminal window.  (On a Mac, this is in Applications > Utilities > Terminal.)
2. Use commands to navigate to the directory you want served. E.g.: `cd ~/Desktop/d3-graphic-hunters`
3. Enter: `python3 -m http.server 8000 &.`
4. Point your browser to: http://localhost:8000/
5. You should now see the contents of that directory in the browser.

Things that could go wrong:

- You don’t have Python installed, so the command isn’t recognized. In that case, install Python from scratch (fun!) or skip ahead to the next section.
- You have Python 2, not 3, installed.  In that case, try this command instead: `python -m SimpleHTTPServer 8000 &.`

### Self-contained Web Server Apps

If the above didn’t work out, for any reason, you may want to download and install a self-contained web server app.  These are standalone pieces of software with graphical user interfaces.

- **Mac** try [MAMP](https://www.mamp.info/en/mac/)
- **Windows** try [WAMPSERVER](https://www.wampserver.com/en/)
- **Any OS** try [XAMPP](https://www.apachefriends.org/download.html) for Linux, Mac, or Windows

Try downloading and following any directions for installation. You'll be done once you can run the web server and have it “serve” out a specific directory to a URL like *localhost:8000* or similar. (The “8000” is just an arbitrary port number; the number itself isn’t important. You just need a local URL that you can point your web browser to.)












