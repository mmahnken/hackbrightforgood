Title: Web App Tutorials
Date: 2014-04-22 1:16
Tags: python, application, tutorial, full-stack
Slug: tutuorials
Category: Tutorials
Authors: Meggie Mahnken
Summary: A collection of tutorials that could be used to make an app for the Hack(bright) for Good Hackathon.

#Web Apps the Hackbright Way

At Hackbright, we teach the microframework for Python web apps called Flask. Flask is a microframework because it doesn't come with a lot of the standard things that frameworks often come with, like an admin interface, an authentication system, an object relational mapper, a testing framework, and the list goes on. It's nice that Flask does not come with those things, because it lets beginner coders learn on their own about what's necessary and good and what is gross garbage.

##About Flask
In a nutshell, Flask is a bunch python functions that have "route decorators" paired with dynamic templating powered by a thing called Jinja. 

A route decorator lets you associate a function in python with a URL ending. In the following example, the route decorator is `@app.route('/mypics')`.
	
	:::python
	@app.route('/mypics')
	def get_pics():
		#do python to get all pictures
		return render_template('pictures.html', pictures = pictures)
	
A user could then go to www.myapp.com/mypics and they would see the template called `pictures.html`. This template knows what these pictures are because we passed it the pictures we obtained in the `get_pics()` function in the `return` statement. See where it says `pictures = pictures`? 

Anyways, it's a bit more complicated than all of that, as you may have guessed. But, if you'd like to give it a try, go [here](http://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world) and do the Hello World exercise (Part 1). 

Next, do the same tutorial's [Part 2](http://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-iv-database) to learn about templates.

##Choose Your Own Flask Adventure
Now that you have the basics down
	
	:::python
	go forth and hack

But seriously, you can do whatever you want at this point. Hopefully you can see that the possibilities are limitless. Here are a mere 3 of them.

###Twitter-like Microblog in Flask
Continue with Miguel Grinberg's comprehensive tutorial of a Microblog (a.k.a. Twitter), but think of your own #hackbrightforgood theme to make it your own. You will learn how to store things in the SQLite database, how to make a profile page with Gravatar avatars, and implement a login system.

 	_Prerequisites: debugging skills, ability to follow written directions carefully, basic command line knowledge_

###To-Do List in Flask
Make a social-good themed to-do list application with Flask using Christian Fernandez's [Tipsy Tutorial](http://chriszf.github.com/tipsy/).

 	_Prerequisites: debugging skills, ability to follow written directions carefully, basic command line knowledge, some knowledge of HTML_

###Instagram App 
Spread happiness and enable creativity by  or make your own instragram filters using [this tutorial by Ajay Kumar N](http://pypix.com/python/instagram-filters-python/) 

 	_Prerequisites: command line knowledge, ability to make your own Flask templates and handlers, intermediate HTML5 knowledge_

###GIF Generator
Happiness is good. If what you hack on makes other people happy... you're hackin' for good. That's my story and I'm sticking to it. If you slightly modify the files from [this tutorial by Zulko](http://zulko.github.io/blog/2014/01/23/making-animated-gifs-from-video-files-with-python/) to take some kind of user input, and then put it into a Flask app, you'd have an instaGIF generator for all to enjoy. 

	_Prerequisites: command line knowledge, ability to make your own Flask templates and handlers, some intermediate HTML5 knowledge_


