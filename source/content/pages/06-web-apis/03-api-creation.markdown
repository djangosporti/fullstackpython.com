title: API Creation
category: page
slug: api-creation
sort-order: 0603
meta: Web APIs enable machine-to-machine communication. Learn more about creating web APIs on Full Stack Python.


# API Creation
Creating and exposing APIs allows your web application to interact with other
applications through machine-to-machine communication.


## API creation frameworks
* [Django REST framework](http://www.django-rest-framework.org/) and
  [Tastypie](https://django-tastypie.readthedocs.org/en/latest/) are 
  the two most widely used API frameworks to use with Django. The edge
  currently goes to Django REST framework based on rough community sentiment.
  Django REST framework continues to knock out great releases after the
  [3.0 release mark](http://www.django-rest-framework.org/topics/3.0-announcement/) 
  when Tom Christie ran a 
  [successful Kickstarter campaign](https://www.kickstarter.com/projects/tomchristie/django-rest-framework-3).

* [Flask-RESTful](http://flask-restful.readthedocs.org/en/latest/) and
  [Flask API](http://www.flaskapi.org/) are popular libraries for 
  exposing APIs from Flask web applications.

* [Sandman](http://www.github.com/jeffknupp/sandman) is a widely used tool to
  automatically generate a RESTful API service from a legacy database without
  writing a line of code (though it's easily extensible through code).

* [Cornice](https://cornice.readthedocs.org/en/latest/) is a REST framework
  for Pyramid.

* [Restless](https://github.com/toastdriven/restless) is a lightweight API
  framework that aims to be framework agnostic. The general concept is that
  you can use the same API code for Django, Flask, Bottle, Pyramid or any
  other WSGI framework with minimal porting effort.

* [Eve](http://python-eve.org/) is a Python REST framework built with Flask,
  MongoDB and Redis. The framework's primary author 
  [Nicola Iarocci](https://twitter.com/nicolaiarocci) gave a great talk at 
  [EuroPython 2014](https://www.youtube.com/watch?v=9sUsLvG72_o) that 
  introduced the main features of the framework.


## API testing projects
Building, running and maintaining APIs requires as much effort as building,
running and maintaining a web application. API testing frameworks are the 
equivalent of browser testing in the web application world.

* [zato-apitest](https://github.com/zatosource/zato-apitest) invokes HTTP 
  APIs and provides hooks for running through other testing frameworks.



## Hosted API testing services
* [Runscope](https://www.runscope.com/) is an API testing SaaS application
  that can test both your own APIs and external APIs that your application
  relies upon.

* [API Science](https://www.apiscience.com/) is focused on deep API testing,
  including multi-step API calls and monitoring of external APIs.

* [SmartBear](http://smartbear.com/api-testing/) has several API monitoring
  and testing tools for APIs.


## API creation resources
* [An API is only as good as its documentation](https://rocketeer.be/blog/2015/03/api-quality/)
  is a strongly held mantra in the web API world because so many APIs have
  poor documentation that prevents ease-of-use. If an API is not well 
  documented then developers who have options to use something else will
  just skip it.

* [10 Reasons Why Developers Hate Your API (And what to do about it)](http://www.slideshare.net/jmusser/ten-reasons-developershateyourapi)
  goes through the top difficulties and annoyances developers face when
  working with APIs and how you can avoid your API falling into the same
  traps.

* Versioning of RESTful APIs is a difficult and contentious topic in the 
  web API community. This two-part series covers 
  [various ways to version your API](http://urthen.github.io/2013/05/09/ways-to-version-your-api/) 
  and [how to architect a version-less API](http://urthen.github.io/2013/05/16/ways-to-version-your-api-part-2/).

* [NARWHL](http://www.narwhl.com/) is a practical API design site for 
  developers confused about what is appropriate for RESTful APIs.

* [18F](https://18f.gsa.gov/)'s 
  [API standards](https://github.com/18f/api-standards) explains the details
  behind their design decisions on creating modern RESTful APIs.

* [Design a beautiful REST API](https://medium.com/@zwacky/design-a-beautiful-rest-api-901c73489458)
  reviews common design decisions regarding endpoints, versioning, errors and
  pagination. There is also a 
  [source material YouTube video](https://www.youtube.com/watch?v=5WXYw4J4QOU)
  where this blog post derives its recommendations from.

* [Move Fast, Don't Break Your API](http://amberonrails.com/move-fast-dont-break-your-api/)
  are slides and a detailed blog post from Amber Feng at Stripe about 
  building an API, separating layers of responsibility, hiding backwards
  compatibility and a whole slew of other great advice for developers
  and API designers.

* [Self-descriptive, isn't. Don't assume anything.](http://www.bizcoder.com/self-descriptive-isn-t-don-t-assume-anything)
  is an appeal that metadata makes a difference in whether APIs are descriptive
  or not.

* [Designing the Artsy API](http://artsy.github.io/blog/2014/09/12/designing-the-public-artsy-api/)
  has their recommendations list for building an API based on their recent
  experiences.

* [Some REST Best Practices](https://bourgeois.me/rest/) is a high level
  summary of rules to follow while creating your API.

* Hacker News had a discussion on 
  [what's the best way to write an API spec?](https://news.ycombinator.com/item?id=8912897)
  that provides a few different viewpoints on this topic.

* [Apigee's Web API Design ebook](https://pages.apigee.com/rs/apigee/images/api-design-ebook-2012-03.pdf)
  is free and contains a wealth of practical advice for what design
  decisions to make for your web API.

* [1-to-1 Relationships and Subresources in REST APIs](http://developers.lyst.com/2015/02/20/1-to-1-relationships-and-subresources-in-rest-apis/)
  tells the story of design decisions that were made during an API's creation
  and why those choices were made.

* [How many status codes does your API need?](https://blogs.dropbox.com/developers/2015/04/how-many-http-status-codes-should-your-api-use/)
  gives an answer from a Dropbox API developer as to their decision making
  process.

* This [API Design Guide](https://github.com/interagent/http-api-design) 
  is based on Heroku's best practices for the platform's API.


## Python-specific API creation resources
* [Choosing an API framework for Django](http://pydanny.com/choosing-an-api-framework-for-django.html)
  by [PyDanny](https://twitter.com/pydanny) contains questions and insight
  into what makes a good API framework and which one you should currently
  choose for Django.

* [Create a REST API in Minutes with Pyramid and Ramses](https://realpython.com/blog/python/create-a-rest-api-in-minutes-with-pyramid-and-ramses/)
  is a thorough tutorial from start to finish that uses the 
  [Pyramid](/pyramid.html) web framework along with 
  [Ramses](https://pypi.python.org/pypi/ramses/), a library that uses
  YAML files to generate a RESTful API.

* [RESTful web services with Python](http://www.slideshare.net/Solution4Future/python-restful-webservices-with-python-flask-and-django-solutions)
  is an interesting overview of the Python API frameworks space.

* [Implementing a RESTful Web API with Python & Flask](http://blog.luisrei.com/articles/flaskrest.html)
  is a good walkthrough for coding a Flask app that provides standard 
  web API functionality such as proper HTTP responses, authentication
  and logging.

* [REST Hooks](http://resthooks.org/) is an open source Python project that 
  makes it easier to implement subscription-based "REST hooks". These REST
  hooks are similar to webhooks, but provide a different mechanism for 
  subscribing to updates via a REST interface. Both REST hooks and webhooks
  are far more efficient than polling for updates and notifications.

* Serialization is common for transforming objects into web API JSON
  results. One company found the serialization performance of Django REST 
  framework was lacking so they created 
  [Serpy](https://github.com/clarkduvall/serpy) and 
  [wrote a blog post with the results of its performance](https://engineering.betterworks.com/2015/09/04/ditching-django-rest-framework-serializers-for-serpy/).


## API creation learning checklist
1. Pick an API framework appropriate for your web framework. For Django I 
   recommend Django REST framework and for Flask I recommend Flask-RESTful.

1. Begin by building out a simple use case for the API. Generally the use 
   case will either involve data that users want in a machine-readable 
   format or a backend for alternative clients such as an iOS or Android 
   mobile app.

1. Add an authentication mechanism through OAuth or a token scheme.

1. Add rate limiting to the API if data usage volume could be a performance 
   issue. Also add basic metrics so you can determine how often the API is 
   being accessed and whether it is performing properly.

1. Provide ample documentation and a walkthrough for how the API can be 
   accessed and used.

1. Figure out other use cases and expand based on what you learned with the 
   initial API use case.

