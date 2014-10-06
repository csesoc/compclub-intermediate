Web Dev
=======

How does a server work?
-----------------------
When you go to a web page in your browser, what's really happening is that your
computer has sent a request for a page to a server, and the server has sent back
the contents of the page. The page is almost always written in HTML. Your web
browser then renders the HTML code to be the pretty page that you see.

A request is usually made up of three parts: the protocol ("http"), the server
name ("www.google.com") and the file name ("index.html"). Your browser sends a
GET request to the server, and the server replies with the contents of the file
requested.

You can see this with the public_html directory that the CSE lab machines have.

When we do web dev, we tend to use existing code to make our lives easier. We
can do simple pages, or bigger projects. For large projects, we use web
development frameworks. For CompClub, we'll be using Python's Flask
microframework.

We can set up routes for the server. On the back-end, we have Python code which
runs like normal, and then decides on an action to perform. The server can
render an HTML page (called a "template"), or redirect to another page.

The server can deal with all normal requests. You're likely to use GET and POST
requests for the web dev project.

We'll look at HTML, CSS (and then Bootstrap), and jQuery.

Project Ideas
-------------

1. A blog
2. Shareable TODO lists
3. Service requests (find someone to mow your lawn or tutor your children)
4. A discussion forum
5. If you have any other ideas, go for it! Just double-check with us first.
