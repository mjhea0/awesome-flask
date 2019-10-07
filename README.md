<div align="center">
  <a href="https://github.com/sindresorhus/awesome#readme"><img src="https://awesome.re/badge-flat.svg" /></a>
  <a href="https://travis-ci.org/mjhea0/awesome-flask"><img src="https://api.travis-ci.org/mjhea0/awesome-flask.svg?branch=master" alt="Build Status" /></a></p>
  <a href="https://twitter.com/intent/tweet?text=Awesome%20Flask%20-%20a%20curated%20list%20of%20awesome%20things%20related%20to%20Flask%20https%3A//github.com/mjhea0/awesome-flask%20%23webdev">Share on Twitter</a>
  <br /><br />
  <img width="400" src="flask-logo.svg" alt="Flask logo">
</div>

# Awesome Flask

> A curated list of awesome things related to Flask, based on [Awesome Django](https://github.com/wsvincent/awesome-django).

## Contents

- [Third-Party Extensions](#third-party-extensions)
  - [Admin](#admin)
  - [APIs](#apis)
  - [Auth](#auth)
  - [Cache](#cache)
  - [Databases](#databases)
  - [Developer Tools](#developer-tools)
  - [Email](#email)
  - [Forms](#forms)
  - [Full-text Search](#full-text-search)
  - [Security](#security)
  - [Task Queues](#task-queues)
  - [Utils](#utils)
- [Resources](#resources)
  - [Official](#official-resources)
  - [External](#external-resources)
  - [Community](#community)
  - [Conferences](#conferences)
    - [Conference Videos from PyVideo.org](#conference-videos-from-pyvideoorg)
  - [Meetups](#meetups)
  - [Podcasts](#podcasts)
  - [Tutorials](#tutorials)
  - [Courses](#courses)
  - [Books](#books)
  - [Videos](#videos)
- [Hosting](#hosting)
  - [PaaS](#paas)
  - [IaaS](#iaas)
  - [Serverless](#serverless)
- [Projects](#Projects)
  - [Boilerplate](#boilerplate)
  - [Open Source Projects](#open-source-projects)

## Third-Party Extensions

### Admin

- [Flask-Admin](https://github.com/flask-admin/flask-admin) - Functional admin panel that provides a user interface for managing data based on your models

### APIs

#### RESTful API Support


- [Flask-RESTful](https://flask-restful.readthedocs.io)
- [Flask-Classful](http://flask-classful.teracy.org/)
- [Flask-MongoRest](https://github.com/closeio/flask-mongorest)
- [Eve](https://docs.python-eve.org)

#### RESTful API + Swagger/OpenAPI Documentation Support

- [Flask-RESTPlus](https://flask-restplus.readthedocs.io)
- [Connexion](https://connexion.readthedocs.io)
- [Flask-Rebar](https://github.com/plangrid/flask-rebar)

#### Swagger/OpenAPI Documentation Support

- [Flask-APISpec](https://flask-apispec.readthedocs.io/en/latest/)

#### Serialization

- [Flask-Marshmallow](https://flask-marshmallow.readthedocs.io)

### Auth

#### Basic (for HTML Endpoints)

- [Flask-Login](https://flask-login.readthedocs.io/) - Account management and authentication
- [Flask Principal](https://pythonhosted.org/Flask-Principal/) - Authorization
- [Flask-HTTPAuth](https://flask-httpauth.readthedocs.io) - Authentication
- [Flask-Security](https://pythonhosted.org/Flask-Security/) - Account management, authentication, authorization
- [Flask-User](https://flask-user.readthedocs.io) - Account management, authentication, authorization

> Curious about the differences differences between Flask-User and Flask-Security? Review the Flask-User [FAQ](https://flask-user.readthedocs.io/en/latest/faq.html).

#### JWT-based (for JSON Endpoints)

- [Flask-Praetorian](https://flask-praetorian.readthedocs.io) - Authentication and authorization for Flask APIs
- [Flask-JWT](https://pythonhosted.org/Flask-JWT/) - Basic support for working with JWTs
- [Flask-JWT-Extended](https://flask-jwt-extended.readthedocs.io) - Advanced support for working with JWTs

#### OAuth

- [Authlib](https://authlib.org/)
- [Authomatic](https://github.com/authomatic/authomatic)
- [Flask-Dance](https://github.com/singingwolfboy/flask-dance)

### Cache

- [Flask-Caching](https://flask-caching.readthedocs.io/) - Caching support

### Databases

- [Flask-SQLAlchemy](https://flask-sqlalchemy.palletsprojects.com) - Support for SQLAlchemy, a SQL toolkit and ORM
- [Flask-Alembic](https://flask-alembic.readthedocs.io) - Configurable Alembic migration environment around a Flask-SQLAlchemy database for handling database migrations
- [Flask-Peewee](https://flask-peewee.readthedocs.io) - Support for Peewee, an ORM and database migration tool
- [Flask-Pony](https://pypi.org/project/Flask-Pony/) - Support for Pony ORM
- [Flask-PyMongo](https://flask-pymongo.readthedocs.io) - Bridges Flask and PyMongo for working with MongoDB
- [Flask-MongoEngine](https://flask-mongoengine.readthedocs.io) - Bridges Flask and MongoEngine for working with MongoDB

### Developer Tools

#### Debugging

- [Flask-DebugToolbar](https://flask-debugtoolbar.readthedocs.io) - Port of Django's debug toolbar for Flask
- [Flask-Profiler](https://github.com/muatik/flask-profiler) - Endpoint analyzer/profiler

#### Fixtures

- [Flask-Fixtures](https://github.com/croach/Flask-Fixtures) - create database fixtures form JSON or YAML
- [Mixer](https://mixer.readthedocs.io) - Object generation tool

#### Logging

- [Rollbar](https://rollbar.com/error-tracking/flask/) - Flask error logging with Rollbar

#### Monitoring

- [Airbrake](https://airbrake.io/docs/installing-airbrake/installing-airbrake-in-a-flask-app/) - Airbrake Flask integration
- [Elastic APM Agent](https://www.elastic.co/guide/en/apm/agent/python/current/flask-support.html) - Elastic APM Flask integration
- [Flask Monitoring Dashboard](https://flask-monitoringdashboard.readthedocs.io) - Dashboard for automatic monitoring of Flask web-services
- [Sentry Python SDK](https://sentry.io/for/flask/) - Sentry SDK Flask integration

#### Tracing

- [Flask-OpenTracing](https://github.com/opentracing-contrib/python-flask) - OpenTracing instrumentation

#### Testing

- [Flask-Testing](https://pythonhosted.org/Flask-Testing/) - Unittest extensions
- [Pytest-Flask](https://github.com/pytest-dev/pytest-flask) - Pytest support for testing Flask applications

### Email

- [Flask-Mail](https://pythonhosted.org/Flask-Mail/) - Provides simple email sending capabilities

### Forms

- [Flask-WTF](https://flask-wtf.readthedocs.io) - Integrates Flask with WTForms

### Full-text Search

- [SQLAlchemy-Searchable](https://sqlalchemy-searchable.readthedocs.io) - Provides full-text search capabilities for SQLAlchemy models

### Security

- [Flask-Bcrypt](https://flask-bcrypt.readthedocs.io) - Provides bcrypt hashing utilities
- [Flask-CORS](https://flask-cors.readthedocs.io) - Cross Origin Resource Sharing (CORS) handling
- [Flask-SeaSurf](https://github.com/maxcountryman/flask-seasurf/) - Cross-site request forgery (CSRF) prevention
- [Flask-Talisman](https://github.com/GoogleCloudPlatform/flask-talisman) - HTTPS and security headers

### Task Queues

- [Celery](http://www.celeryproject.org/)
- [Dramatiq](https://flask-dramatiq.rtfd.io/)
- [Flask-RQ](https://github.com/mattupstate/flask-rq)
- [Huey](https://huey.readthedocs.io)

### Utils

- [Flask-Babel](https://github.com/python-babel/flask-babel) - Support for internationalization (i18n) and localization (l10n)
- [Flask-FlatPages](https://pythonhosted.org/Flask-FlatPages/) - Provides flat static pages based on text files
- [Frozen-Flask](https://github.com/Frozen-Flask/Frozen-Flask) - Freezes a Flask application into a set of static files
- [Flask-GraphQL](https://github.com/graphql-python/flask-graphql) - GraphQL support
- [Flask-Limiter](https://flask-limiter.readthedocs.io) - Rate limiting features to Flask routes
- [Flask-Moment](https://github.com/miguelgrinberg/Flask-Moment) - Moment.js date and time formatting helpers for Jinja2 templates
- [Flask-Paginate](https://pythonhosted.org/Flask-paginate/) - Pagination support
- [Flask-Sitemap](https://flask-sitemap.readthedocs.io) - Sitemap generation
- [Flask-SocketIO](https://flask-socketio.readthedocs.io) - Socket.IO integration

## Resources

### Official Resources

- [Project Website](https://palletsprojects.com/p/flask/) - Official Flask website
- [Documentation](https://flask.palletsprojects.com) - Comprehensive documentation for all Flask versions
- [Flaskr Tutorial](https://flask.palletsprojects.com/tutorial/) - Build a basic blog application called Flaskr
- [Source Code](https://github.com/pallets/flask) - Hosted on Github

### External Resources

- [TestDriven](https://testdriven.io/blog/) - Up-to-date tutorials on Flask
- [Miguel Grinberg's Blog](https://blog.miguelgrinberg.com/category/Flask) - Multiple Flask-specific tutorials
- [Full Stack Python's Flask Page](https://www.fullstackpython.com/flask.html) - Explanation of Flask philosophy and links to other resources and tutorials
- [RealPython](https://realpython.com/tutorials/flask/) - Many high-quality tutorials on Flask
- [Patrick Kennedy's Blog](http://www.patricksoftwareblog.com/flask-tutorial/) - Numerous tutorials on learning Python web application development with Flask
- [Nick Janetakis's Blog](https://nickjanetakis.com/blog/tag/flask-tips-tricks-and-tutorials) - Flask Tips, Tricks and Tutorials

### Community

- [Mailing List](https://mail.python.org/mailman/listinfo/flask) (`flask@python.org`) - General discussion of Flask and the Pallets projects
- [Discord](https://discordapp.com/invite/t6rrQZH) - Pallets Projects community on Discord (use the `#get-help` channel for Flask support)
- [Twitter](https://twitter.com/palletsteam) - For official announcements on updates, security fixes, etc.
- [Stack Overflow](https://stackoverflow.com/questions/tagged/flask) - Questions tagged `flask`
- [Reddit](https://www.reddit.com/r/flask/) - Flask subreddit
- IRC Channel - Chat with other Flask users on IRC channel `#pocoo` on FreeNode
- [Flask Jobs](https://flaskjobs.com) - A job board dedicated to Flask.

### Conferences

- [PyConWeb](https://pyconweb.com/)
- [Flask Conf Brazil](https://2019.flask.python.org.br/)
- [PyCon US](https://us.pycon.org/2019/)
- [PyCon Australia](https://2019.pycon-au.org/)
- [Euro Python](https://ep2019.europython.eu/)
- [Complete listing of all PyCons globally](https://pycon.org/)

#### Conference Videos from PyVideo.org

- [Flask Conf Brazil - 2018](https://pyvideo.org/events/flask-conf-2018.html)
- [PyCon US - 2019](https://pyvideo.org/events/pycon-us-2019.html)
- [EuroPython - 2019](https://pyvideo.org/events/europython-2019.html)
- [PyCon Australia - 2019](https://pyvideo.org/events/pycon-au-2019.html)
- [Complete listing of videos](https://pyvideo.org/events.html)

### Meetups

- [Flask](https://www.meetup.com/topics/flask/all/) - 40+ groups in 20 countries
- [Python Web Development](https://www.meetup.com/topics/python-web-development/all/) - 600+ groups in 81 countries
- [Python](https://www.meetup.com/topics/python/all/) - 2,400+ groups in 100 countries

### Podcasts

- [TalkPython](https://talkpython.fm/) - The leading Python podcast with several episodes on Flask
- [Podcast Init](https://www.pythonpodcast.com/) - A popular Python podcast that features Flask guests on occasion
- [Python Bytes](https://pythonbytes.fm/) - Another Python podcast that discusses Flask from time to time
- [Full Stack Python's Best Python Podcasts Page](https://www.fullstackpython.com/best-python-podcasts.html) - A list of active Python-specific podcasts

### Tutorials

- [The Flask Mega-Tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world)
- [Intro to Flask, Test-Driven Development (TDD), and JavaScript](https://github.com/mjhea0/flaskr-tdd)
- [Make a Web App Using Python & Flask!](https://aryaboudaie.com/python/technical/educational/web/flask/2018/10/17/flask.html)

### Courses

- [Test-Driven Development with Python, Flask, and Docker](https://testdriven.io/courses/tdd-flask/)
- [Authentication with Flask, React, and Docker](https://testdriven.io/courses/auth-flask-react/)
- [Deploying a Flask and React Microservice to AWS ECS](https://testdriven.io/courses/aws-flask-react/)
- [Build a SAAS App with Flask](https://buildasaasappwithflask.com)
- [Full Stack Foundations](https://www.udacity.com/course/full-stack-foundations--ud088)
- [Designing RESTful APIs](https://www.udacity.com/course/designing-restful-apis--ud388)

### Books

- [Flask Web Development](https://www.oreilly.com/library/view/flask-web-development/9781491991725/)
- [Real Python](https://realpython.com)
- [Explore Flask](https://exploreflask.com/)

### Videos

- [PyVideo](https://pyvideo.org/search.html?q=flask)
- [Practical Flask Web Development Tutorials](https://www.youtube.com/playlist?list=PLQVvvaa0QuDc_owjTbIY4rbgXOFkUYOUB)
- [Python Flask Tutorial: Full-Featured Web App](https://www.youtube.com/playlist?list=PL-osiE80TeTs4UjLw5MM6OjgkjFeUxCYH)
- [Discover Flask - Full Stack Web Development with Flask](https://github.com/realpython/discover-flask)

## Hosting

### PaaS

(Platforms-as-a-Service)

- [Heroku](https://www.heroku.com/)
- [PythonAnywhere](https://www.pythonanywhere.com/details/flask_hosting)
- [AWS Elastic Beanstalk](https://aws.amazon.com/elasticbeanstalk/)
- [Google App Engine](https://cloud.google.com/appengine/)
- [Microsoft Azure App Service](https://azure.microsoft.com/services/app-service/)
- [Divio](https://www.divio.com)
- [Render](https://render.com/)

### IaaS

(Infrastructure-as-a-Service)

- [AWS EC2](https://aws.amazon.com/ec2/)
- [Google Compute Engine](https://cloud.google.com/compute/)
- [Digital Ocean](https://www.digitalocean.com/)
- [Linode](https://www.linode.com/)

### Serverless

Frameworks:

- [Zappa](https://github.com/Miserlou/Zappa)
- [Chalice](https://github.com/aws/chalice)

Compute:

- [AWS Lambda](https://aws.amazon.com/lambda/)
- [Google Cloud Functions](https://cloud.google.com/functions/)

## Projects

### Boilerplate

- [cookiecutter-flask](https://github.com/cookiecutter-flask/cookiecutter-flask)
- [Cookiecutter Flask Skeleton](https://github.com/realpython/cookiecutter-flask-skeleton)
- [gae-init](https://gae-init.appspot.com) - For starting new applications on Google App Engine
- [Flask-AppBuilder](https://github.com/dpgaspar/Flask-AppBuilder)
- [flask-base](http://hack4impact.github.io/flask-base/)
- [Flask-Bootstrap](https://github.com/esbullington/flask-bootstrap)
- [uwsgi-nginx-flask-docker](https://github.com/tiangolo/uwsgi-nginx-flask-docker) - Docker image with uWSGI and Nginx for Flask applications in Python running in a single container
- [React-Redux-Flask](https://github.com/dternyak/React-Redux-Flask)
- [Flask-Scaffold](https://github.com/Leo-G/Flask-Scaffold)

### Open Source Projects

- [Redash](https://github.com/getredash/redash)
- [Airflow](https://github.com/apache/airflow/tree/master/airflow/www)
- [FlaskBB](https://github.com/flaskbb/flaskbb)
- [Indico](https://github.com/indico/indico)
- [Quokka CMS](http://quokkaproject.org/)
- [SkyLines](https://github.com/skylines-project/skylines)
- [Timesketch](https://github.com/google/timesketch)
- [Security Monkey](https://github.com/Netflix/security_monkey)
- [SecureDrop](https://github.com/freedomofpress/securedrop)
- [PythonBuddy](https://github.com/ethanchewy/PythonBuddy)
- [Busy Beaver](https://github.com/busy-beaver-dev/busy-beaver)

---

<br>

> **NOTE**: This tutorial is powered by **[TestDriven.io](https://testdriven.io/)**. Please support this open source project by purchasing one of our Flask courses. Learn how to build, test, and deploy microservices powered by Docker, Flask, and React!
