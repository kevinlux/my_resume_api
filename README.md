# My Resume/CV API

<img src="./gopher.png" width="300">

This is an API written in Go using the Gin web framework. The API gets my resume (stored as JSON in a MongoDB instance) and returns it to the user, either in full or by section. If you access the website at the root directory it will  return a JSON object containing all the resume data. If you go to "/resume.html" you get to see my resume as an HTML document. You can also get a certain section of a resume by accessing "/{{section}}". For instance, you can get a JSON object containing only the technologies via a GET request to "/technologies". The resume JSON in the database can also be updated via PUT request to the root directory. However, I have protected this with a token so that I'm the only one who can update it.

This used to be hosted on Heroku when they had the free tier
