# 💥💥 Site-reservation-artist-Fyyur
<mark> Udacity - Full Stack Web Developer 👨‍💻 Nanodegree Project 01 </mark>
-----

### Introduction

Fyyur is a music site and an artist booking site that simplifies the discovery and booking of shows between local artists and clubs. This site allows you to list new artists and places, discover them and list shows with artists as the owner of the place.

Your job is to build data models to power the API endpoints for the Fyyur site by connecting to a PostgreSQL database to store, query and create information about artists and places in Fyyur.

### Overview

This application is almost complete. Only one thing is missing ... real data! Although views and controllers are defined in this application, models and interactions between models to store, retrieve and update data from a database are missing. At the end of this project, you should have a fully functional site that is at least capable of doing the following, if not more, using a PostgreSQL database:

* creation of new places, artists and creation of new shows.
* Search for places and artists.
* Learn more about a specific artist or location.

We want Fyyur to be the next new platform that artists and music venues can use to meet and discover new musical performances. Let's make it happen!

### Technological stack

Our technology stack will include:

* ** SQLAlchemy ORM ** will be our favorite ORM library
* ** PostgreSQL ** as our favorite database
* ** Python3 ** and ** Flask ** as the language of our server and server framework
* ** Flask-Migrate ** to create and migrate schemas
* ** HTML **, ** CSS ** and ** Javascript ** with [Bootstrap 3] (https://getbootstrap.com/) for the interface of our website

### Main files: structure of the project

  `` 'sh
  ├── README.md
  ├── app.py *** the main application controller. Include your SQLAlchemy models.
                    "python app.py" to run after installing dependencies
  ├── config.py *** database URL, CSRF generation, etc.
  ├── error.log
  ├── forms.py *** Your forms
  ├── require.txt *** The dependencies we need to install with "pip3 install -r require.txt"
  ├── static
  │ ├── css
  Source │ ├──
  │ ├── ico
  │ ├── img
  │ └── js
  └── models
      ├── errors
      ├── forms
      ├── drawings
      └── pages
  `` ''

Generally:
* The models can be found in the `MODELS` section of the` app.py`.
* The drivers are also found in `app.py`.
* The web interface is located in `templates /`, which creates static resources implemented on the web server in `static /`.
* The web forms for creating data are in `form.py`


Highlight folders:
* `templates / pages` - (Already completed.) Defines the pages that are displayed on the site. These models represent views based on the data passed to the model view, in the drivers defined in `app.py`. These pages correctly represent your data and are already defined for you.
* `templates / layout` - (already completed). Defines the layout in which a page can be contained to define the footer and header code for a given page.
* `models / modules` - (already completed). Define the modules used to create new artists, shows and places.
* `app.py` - (Functionality missing). It defines paths that correspond to the user's URL and drivers that manage data and display views to the user. This is the main file in which you will work to connect and manipulate the database and view the views with data to the user, based on the URL.
* Models in `app.py` - (Lack of functionality). Defines the data models that configure the database tables.
* `config.py` - (Missing functionality). Stores configuration variables and instructions, separate from the main application code. Here you need to connect to the database.


Instructions
-----

1. Understand the project structure (explained above) and the location of important files.
2. Create and run local development by following the Development configuration steps below.
3. Enter the missing features in this app: this app is currently extracting fake data and now you have to connect to a real database and talk to a real backend.
3. Complete each `TODO` section in the whole code base. We suggest you go in the following order:

  1. Connect to a database in `config.py`. A project submission that uses a connection to the local database is fine.
  2. Using SQLAlchemy, configure normalized models for the objects we support in our web application in the Models section of `app.py`. See the pages of
