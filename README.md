# Awesome Flask [![Awesome](https://awesome.re/badge-flat.svg)](https://github.com/sindresorhus/awesome)

> A curated list of awesome things related to Flask.

<!--lint ignore double-link-->
[Flask](https://flask.palletsprojects.com/) is a lightweight WSGI web application framework written in Python.

## Contents

- [Third-Party Extensions](#third-party-extensions)
  - [Admin](#admin)
  - [APIs](#apis)
  - [Auth](#auth)
  - [Cache](#cache)
  - [Data Validation and Serialization](#data-validation-and-serialization)
  - [Databases](#databases)
  - [Developer Tools](#developer-tools)
  - [Email](#email)
  - [Forms](#forms)
  - [Full-text Search](#full-text-search)
  - [Security](#security)
  - [Task Queues](#task-queues)
  - [Utils](#utils)
- [Resources](#resources)
  - [Official Resources](#official-resources)
  - [External Resources](#external-resources)
  - [Community](#community)
  - [Conferences](#conferences)
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
- [Projects](#projects)
  - [Boilerplates](#boilerplates)
  - [Open Source Projects](#open-source-projects)

## Third-Party Extensions

### Admin

- [Flask-Admin](https://github.com/flask-admin/flask-admin) - Functional admin panel that provides a user interface for managing data based on your models.

### APIs

#### RESTful API Support

- [Eve](https://docs.python-eve.org) - RESTful API framework designed for human beings.
- [Flask-Classful](https://flask-classful.teracy.org/) - Adds support for class-based views for setting up RESTful API route endpoints.
- [Flask-MongoRest](https://github.com/closeio/flask-mongorest) - RESTful API framework wrapped around [MongoEngine](http://mongoengine.org/).
- [Flask-RESTful](https://flask-restful.readthedocs.io) - Quickly build RESTful APIs.

#### RESTful API + Swagger/OpenAPI Documentation Support

- [Connexion](https://connexion.readthedocs.io) - Open source, OpenAPI-based, REST framework built on top of Flask.
- [Flask-Rebar](https://github.com/plangrid/flask-rebar) - Combines Flask, [marshmallow](https://marshmallow.readthedocs.io/), and [OpenAPI](https://www.openapis.org/) for robust REST services.
- [Flask-RESTX](https://flask-restx.readthedocs.io) - Community-driven fork of [Flask-RESTPlus](https://flask-restplus.readthedocs.io/) that makes it easy to build and document RESTful APIs with Flask.

#### Swagger/OpenAPI Documentation Support

- [Flask-APISpec](https://flask-apispec.readthedocs.io/) - Auto-documenting REST APIs.
- [SAFRS: Python OpenAPI & JSON:API Framework](https://github.com/thomaxxl/safrs) - SAFRS, which is an acronym for *S*ql*A*lchemy *F*lask-*R*estful *S*wagger, is meant to help developers create self-documenting JSON APIs for SQLAlchemy database objects and relationships.

### Auth

#### Basic Auth and Session-based (for HTML Endpoints)

- [Flask-HTTPAuth](https://flask-httpauth.readthedocs.io) - Authentication.
- [Flask-Login](https://flask-login.readthedocs.io/) - Account management and authentication.
- [Flask Principal](https://pythonhosted.org/Flask-Principal/) - Authorization.
- [Flask-Security-Too](https://flask-security-too.readthedocs.io/en/stable/) - Account management, authentication, authorization.
- [Flask-SimpleLogin](https://github.com/flask-extensions/Flask-SimpleLogin) - Authentication.
- [Flask-User](https://flask-user.readthedocs.io) - Account management, authentication, authorization.

> Curious about the differences differences between Flask-User and Flask-Security? Review the Flask-User [FAQ](https://flask-user.readthedocs.io/en/latest/faq.html).

#### JWT-based (for JSON Endpoints)

- [Flask-JWT](https://pythonhosted.org/Flask-JWT/) - Basic support for working with JWTs.
- [Flask-JWT-Extended](https://flask-jwt-extended.readthedocs.io) - Advanced support for working with JWTs.
- [Flask-JWT-Router](https://github.com/joegasewicz/flask-jwt-router) - Adds authorized routes to a Flask app.
- [Flask-Praetorian](https://flask-praetorian.readthedocs.io) - Authentication and authorization for Flask APIs.

#### OAuth

- [Authlib](https://authlib.org/) - Library for building OAuth and OpenID clients and servers.
- [Authomatic](https://github.com/authomatic/authomatic) - Framework agnostic library for Python web applications that simplifies authentication and authorization of users via OAuth and OpenID.
- [Flask-Dance](https://github.com/singingwolfboy/flask-dance) - OAuth support via [OAuthLib](https://oauthlib.readthedocs.io/).

### Cache

- [Flask-Caching](https://flask-caching.readthedocs.io/) - Caching support.

### Data Validation and Serialization

- [Flask-Marshmallow](https://flask-marshmallow.readthedocs.io) - Thin integration layer for Flask and marshmallow (an object serialization /deserialization library) that adds additional features to marshmallow.
- [Flask-Pydantic](https://github.com/bauerji/flask-pydantic) - [Pydantic](https://github.com/pydantic/pydantic) support.

### Databases

#### ORMs

- [Flask-Peewee](https://flask-peewee.readthedocs.io) - Support for Peewee, an ORM and database migration tool.
- [Flask-Pony](https://pypi.org/project/Flask-Pony/) - Support for Pony ORM.
- [Flask-SQLAlchemy](https://flask-sqlalchemy.palletsprojects.com) - Support for SQLAlchemy, a SQL toolkit and ORM.

#### ODMs

- [Flask-MongoEngine](https://flask-mongoengine.readthedocs.io) - Bridges Flask and MongoEngine for working with MongoDB.
- [Flask-PyMongo](https://flask-pymongo.readthedocs.io) - Bridges Flask and PyMongo for working with MongoDB.

#### Migrations

- [Flask-Alembic](https://flask-alembic.readthedocs.io) - Configurable [Alembic](https://alembic.sqlalchemy.org/) migration environment around a Flask-SQLAlchemy database for handling database migrations.
<!--lint ignore double-link-->
- [Flask-DB](https://github.com/nickjj/flask-db) - Flask CLI extension that helps you migrate, drop, create and seed your SQL database.
- [Flask-Migrate](https://flask-migrate.readthedocs.io) - Handles SQLAlchemy database migrations via Alembic.

<!--lint ignore double-link-->
> Curious about the differences between Alembic, Flask-Alembic, Flask-Migrate, and Flask-DB? Review [this item](https://github.com/nickjj/flask-db#differences-between-alembic-flask-migrate-flask-alembic-and-flask-db) from Flask-DB's FAQ.

#### Other Tools

- [Flask-Excel](https://github.com/pyexcel-webwares/Flask-Excel) - Uses [pyexcel](https://github.com/pyexcel/pyexcel) to read, manipulate, and write data in different Excel formats: csv, ods, xls, xlsx and xlsm.

### Developer Tools

#### Debugging

- [Flask-DebugToolbar](https://flask-debugtoolbar.readthedocs.io) - Port of Django's debug toolbar for Flask.
- [Flask-Profiler](https://github.com/muatik/flask-profiler) - Endpoint analyzer/profiler.

#### Fixtures

- [Flask-Fixtures](https://github.com/croach/Flask-Fixtures) - Create database fixtures from JSON or YAML.
- [Mixer](https://mixer.readthedocs.io) - Object generation tool.

#### Logging

- [Rollbar](https://rollbar.com/platforms/flask-error-tracking/) - Flask error logging with Rollbar.

#### Monitoring

- [Airbrake](https://docs.airbrake.io/docs/platforms/framework/python/flask/) - Airbrake Flask integration.
- [Elastic APM Agent](https://www.elastic.co/guide/en/apm/agent/python/current/flask-support.html) - Elastic APM Flask integration.
- [Flask Monitoring Dashboard](https://flask-monitoringdashboard.readthedocs.io) - Dashboard for automatic monitoring of Flask web-services.
- [Sentry Python SDK](https://sentry.io/for/flask/) - Sentry SDK Flask integration.

#### Tracing

- [Flask-OpenTracing](https://github.com/opentracing-contrib/python-flask) - OpenTracing instrumentation.

#### Testing

- [Flask-Testing](https://pythonhosted.org/Flask-Testing/) - Unittest extensions.
- [Pytest-Flask](https://github.com/pytest-dev/pytest-flask) - Pytest support for testing Flask applications.

### Email

- [Flask-Mail](https://pythonhosted.org/Flask-Mail/) - Provides simple email sending capabilities.
- [Flask-Mailman](https://pypi.org/project/flask-mailman/) - A port of `django.mail` for Flask.

### Forms

- [Flask-WTF](https://flask-wtf.readthedocs.io) - Integrates Flask with WTForms (provides CSRF protection as well).

### Full-text Search


- [flask-msearch](https://github.com/honmaple/flask-msearch) - Full-text search.
- [Flask-WhooshAlchemy3](https://github.com/blakev/Flask-WhooshAlchemy3) - Full-text search + Whoosh indexing capabilities for Flask-SQLAlchemy.
- [SQLAlchemy-Searchable](https://sqlalchemy-searchable.readthedocs.io) - Provides full-text search capabilities for SQLAlchemy models.

### Security

- [Flask-Bcrypt](https://flask-bcrypt.readthedocs.io) - Provides bcrypt hashing utilities.
- [Flask-CORS](https://flask-cors.readthedocs.io) - Cross Origin Resource Sharing (CORS) handling.
- [Flask-SeaSurf](https://github.com/maxcountryman/flask-seasurf/) - Cross-site request forgery (CSRF) prevention.
- [Flask-Talisman](https://github.com/GoogleCloudPlatform/flask-talisman) - HTTPS and security headers.

### Task Queues

- [Celery](https://docs.celeryproject.org/) - The most commonly used Python library for handling asynchronous tasks and scheduling.
- [Dramatiq](https://flask-dramatiq.rtfd.io/) - Fast and reliable alternative to Celery.
- [Flask-RQ](https://github.com/mattupstate/flask-rq) - [RQ](https://python-rq.org/) (Redis Queue) integration.
- [Huey](https://huey.readthedocs.io) - [Redis](https://redis.io/)-based task queue that aims to provide a simple, yet flexible framework for executing tasks.

### Utils

- [Flask-Babel](https://github.com/python-babel/flask-babel) - Support for internationalization (i18n) and localization (l10n).
- [Flask-File-Upload](https://github.com/joegasewicz/flask-file-upload) - Easy file uploads.
- [Flask-FlatPages](https://pythonhosted.org/Flask-FlatPages/) - Provides flat static pages based on text files.
- [Frozen-Flask](https://github.com/Frozen-Flask/Frozen-Flask) - Freezes a Flask application into a set of static files.
- [Flask-GraphQL](https://github.com/graphql-python/flask-graphql) - GraphQL support.
- [Flask-Injector](https://github.com/alecthomas/flask_injector) - Adds support for dependency injection.
- [Flask-Limiter](https://flask-limiter.readthedocs.io) - Rate limiting features to Flask routes.
- [Flask-Moment](https://github.com/miguelgrinberg/Flask-Moment) - Moment.js date and time formatting helpers for Jinja2 templates.
- [Flask-Paginate](https://pythonhosted.org/Flask-paginate/) - Pagination support.
- [Flask-Reactize](https://github.com/Azure-Samples/flask-reactize) - Hides the Node.js development backend for React behind a Flask application.
- [Flask-Shell2HTTP](https://github.com/Eshaan7/Flask-Shell2HTTP) - RESTful/HTTP wrapper for Python's subprocess API, so you can convert any command-line tool into a RESTful API service.
- [Flask-Sitemap](https://flask-sitemap.readthedocs.io) - Sitemap generation.
- [Flask-SocketIO](https://flask-socketio.readthedocs.io) - Socket.IO integration.

## Resources

### Official Resources

- [Project Website](https://palletsprojects.com/p/flask/) - Official Flask website.
<!--lint ignore double-link-->
- [Documentation](https://flask.palletsprojects.com) - Comprehensive documentation for all Flask versions.
- [Flaskr Tutorial](https://flask.palletsprojects.com/tutorial/) - Build a basic blog application called Flaskr.
- [Source Code](https://github.com/pallets/flask) - Hosted on GitHub.

### External Resources

- [Full Stack Python's Flask Page](https://www.fullstackpython.com/flask.html) - Explanation of Flask philosophy and links to other resources and tutorials.
- [Miguel Grinberg's Blog](https://blog.miguelgrinberg.com/category/Flask) - Multiple Flask-specific tutorials.

- [Nick Janetakis's Blog](https://nickjanetakis.com/blog/tag/flask-tips-tricks-and-tutorials) - Flask Tips, Tricks and Tutorials.
- [Patrick Kennedy's Blog](http://www.patricksoftwareblog.com/flask-tutorial/) - Numerous tutorials on learning Python web application development with Flask.
- [RealPython](https://realpython.com/tutorials/flask/) - Many high-quality tutorials on Flask.
- [TestDriven.io](https://testdriven.io/blog/topics/flask/) - Up-to-date tutorials on Flask.

### Community

- [Discord](https://discord.com/invite/t6rrQZH) - Pallets Projects community on Discord (use the `#get-help` channel for Flask support).
- IRC Channel - Chat with other Flask users on IRC channel `#pocoo` on FreeNode.
- [Mailing List](https://mail.python.org/mailman/listinfo/flask) - General discussion of Flask and the Pallets projects (`flask@python.org`).
- [Reddit](https://www.reddit.com/r/flask/) - Flask subreddit.
- [Stack Overflow](https://stackoverflow.com/questions/tagged/flask) - Questions tagged `flask`.
- [Twitter](https://twitter.com/PalletsTeam) - For official announcements on updates, security fixes, etc.

### Conferences

- [FlaskCon](https://twitter.com/flaskcon) - Community driven Flask event intended for speakers and attendees all over the world to participate in technical and evangelical sessions related to Flask.
- [PyConWeb](https://twitter.com/pyconweb) - Covers Django, Tornado, Flask, API frameworks. AsyncIO, networking, Frontend, JavaScript, and web security.
- [Flask Conf Brazil](https://2019.flask.python.org.br/) - Conference for the developers and users of Flask.
- [PyCon US](https://us.pycon.org/) - The largest annual gathering for the community using and developing the open-source Python programming language.
- [PyCon Australia](https://pycon-au.org/) - National conference organized for the Python Programming Community.
- [Euro Python](https://europython.eu/) - The largest Python conference in Europe.
- [PyCon](https://pycon.org/) - Complete listing of all PyCons globally.

### Meetups

- [Flask](https://www.meetup.com/topics/flask/all/) - 40+ groups in 20 countries.
- [Python Web Development](https://www.meetup.com/topics/python-web-development/all/) - 600+ groups in 81 countries.
- [Python](https://www.meetup.com/topics/python/all/) - 2,400+ groups in 100 countries.

### Podcasts

- [TalkPython](https://talkpython.fm/) - The leading Python podcast with several episodes on Flask.
- [Podcast Init](https://www.pythonpodcast.com/) - A popular Python podcast that features Flask guests on occasion.
- [Python Bytes](https://pythonbytes.fm/) - Another Python podcast that discusses Flask from time to time.
- [Full Stack Python's Best Python Podcasts Page](https://www.fullstackpython.com/best-python-podcasts.html) - A list of active Python-specific podcasts.

### Tutorials

- [Flask Mega-Tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world) - Overarching tutorial for Python beginner and intermediate developers that teaches web development with the Flask framework.
- [Flaskr TDD](https://github.com/mjhea0/flaskr-tdd) - Intro to Flask, Test-Driven Development (TDD), and JavaScript.
- [Make a Web App Using Python & Flask!](https://aryaboudaie.com/python/technical/educational/web/flask/2018/10/17/flask.html) - Creating a Python Website from the Bottom Up.

### Courses

- [Developing Web Applications with Python and Flask](https://testdriven.io/courses/learn-flask/) - This course focuses on teaching the fundamentals of Flask by building and testing a web application using Test-Driven Development (TDD).
- [Test-Driven Development with Python, Flask, and Docker](https://testdriven.io/courses/tdd-flask/) - Learn how to build, test, and deploy a production-grade microservice powered by Python, Flask, and Docker.
- [Authentication with Flask, React, and Docker](https://testdriven.io/courses/auth-flask-react/) - Learn how to add authentication to a Flask and React microservice!.
- [Deploying a Flask and React Microservice to AWS ECS](https://testdriven.io/courses/aws-flask-react/) - Learn how to deploy microservices to Amazon ECS powered by Flask, React, and Docker.
- [Build a SAAS App with Flask](https://buildasaasappwithflask.com) - Learn to build web applications with Flask and Docker.
- [Full Stack Foundations](https://www.udacity.com/course/full-stack-foundations--ud088) - Build a data-driven web app with Python.
- [Designing RESTful APIs](https://www.udacity.com/course/designing-restful-apis--ud388) - Build and Secure a backend API server.

### Books

- [Flask Web Development](https://www.oreilly.com/library/view/flask-web-development/9781491991725/) - Learn the framework from the ground up by developing, step-by-step, a real-world project.
- [Real Python](https://realpython.com) - Learn Python programming, by example.
- [Explore Flask](https://exploreflask.com/) - Best practices and patterns for developing web applications with Flask.

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
- [Microsoft Azure App Service](https://azure.microsoft.com/en-us/services/app-service/)
- [Divio](https://www.divio.com)
- [Render](https://render.com/)

### IaaS

(Infrastructure-as-a-Service)

- [AWS EC2](https://aws.amazon.com/ec2/)
- [Google Compute Engine](https://cloud.google.com/compute/)
- [Digital Ocean](https://www.digitalocean.com/)
<!-- markdown-link-check-disable-next-line -->
- [Linode](https://www.linode.com/)

### Serverless

Frameworks:

- [Zappa](https://github.com/Miserlou/Zappa)
- [Chalice](https://github.com/aws/chalice)

Compute:

- [AWS Lambda](https://aws.amazon.com/lambda/)
- [Google Cloud Functions](https://cloud.google.com/functions/)
- [Azure Functions](https://azure.microsoft.com/en-us/services/functions/)

## Projects

### Boilerplates

- [cookiecutter-flask](https://github.com/cookiecutter-flask/cookiecutter-flask) - With Bootstrap 4, asset bundling annd minification with webpack, starter templates, and registration/authentication.
- [Cookiecutter Flask Skeleton](https://github.com/testdrivenio/cookiecutter-flask-skeleton) - Flask starter project for [Cookiecutter](https://github.com/cookiecutter/cookiecutter).
- [Flask-AppBuilder](https://github.com/dpgaspar/Flask-AppBuilder) - Simple and rapid application development framework that includes detailed security, auto CRUD generation for your models, Google charts, and much more.
- [flask-base](http://hack4impact.github.io/flask-base/) - Includes SQLAlchemy, Redis, User Authentication, and more.
- [Flask-Bootstrap](https://github.com/esbullington/flask-bootstrap) - Integrated SQLAlchemy, authentication, and Bootstrap frontend.
- [uwsgi-nginx-flask-docker](https://github.com/tiangolo/uwsgi-nginx-flask-docker) - Docker image with uWSGI and Nginx for Flask applications in Python running in a single container.
- [React-Redux-Flask](https://github.com/dternyak/React-Redux-Flask) - Boilerplate application for a Flask JWT Backend and a React/Redux Front-End with Material UI.
- [Flask-Scaffold](https://github.com/Leo-G/Flask-Scaffold) - Prototype Database driven Web apps in Angular 6, Bootstrap 4 and REST API's with Flask.
- [Flask-VueJS](https://github.com/marcuxyz/flask-vuejs) - Connect Flask application with VueJS.
- [Flask-Backbone](https://github.com/abstractkitchen/flask-backbone) - Flask Boilerplate with an optional SQLAlchemy and other tools out of the box.

### Open Source Projects

- [ActorCloud](https://github.com/actorcloud/ActorCloud) - Open-source IoT Platform.
- [Airflow](https://github.com/apache/airflow/tree/master/airflow/www)
- [Busy Beaver](https://github.com/busy-beaver-dev/busy-beaver) - Chicago Python's Community Engagement Slack bot.
- [FlaskBB](https://github.com/flaskbb/flaskbb) - Classic forum software.
- [Indico](https://github.com/indico/indico) - Feature-rich event management system, made at [CERN](https://home.cern/).
- [Quokka CMS](https://github.com/quokkaproject) - The happiest CMS in the world.
- [PythonBuddy](https://github.com/ethanchewy/PythonBuddy) - Online Python Editor with live syntax checking and execution.
- [Redash](https://github.com/getredash/redash) - Designed to enable anyone, regardless of the level of technical sophistication, to harness the power of data big and small.
- [SkyLines](https://github.com/skylines-project/skylines) - Live tracking, flight database, and competition framework.
- [Security Monkey](https://github.com/Netflix/security_monkey) - Monitors AWS, GCP, OpenStack, and GitHub orgs for assets and their changes over time.
- [SecureDrop](https://github.com/freedomofpress/securedrop) - Open-source whistleblower submission system that media organizations can use to securely accept documents from, and communicate with anonymous sources.
- [SimpleLogin](https://github.com/simple-login/app) - Protect your online identity with email alias.
- [sr.ht](https://git.sr.ht/~sircmpwn/core.sr.ht/tree) - Git hosting service (check out [Why I chose Flask to build sr.ht's mini-services](https://drewdevault.com/2019/01/30/Why-I-built-sr.ht-with-Flask.html) as well).
- [Timesketch](https://github.com/google/timesketch) - Collaborative forensic timeline analysis.

---

<br>

> **NOTE**: This project is powered by **[TestDriven.io](https://testdriven.io/)**. Please support this open source project by purchasing one of our Flask courses. Learn how to build, test, and deploy microservices powered by Docker, Flask, and React!
