![image](http://dreamsofpy.github.io/assets/img/slider/slider2.jpg)
Style_for_Engineers (Mens edition)
===================

Geek Quarterly #DressedToCode

A geek version of GQ; helping engineers choose occasion appropriate outfits based on fit and style, for when they are ready to step away from their desk. To help them stay current on brands and styles relevant to the outside world, this app will take some information from APIs and condense them into executive summary style reports. Elements of this project include big data, semantic analysis, and visualizations.

Tasks:

* **Architecture:**
    * Content for the resume; sections can include qualifications, quantified levels, responsibilities, technical environment, location, industry
    * Decide how user will enter in information such as occasion (work, formal event, etc.)
    * Make it easy to rate yes or no
* **Data-Scientists:**
    * Run analysis on mens clothing items
        * Find mens clothing objects (i.e. khakis, loafers, tie, etc)
        * Measure sentiment in each mention, is it positive or negative?
* **Back-End:**
    * Create and set up api wrappers for social fashion sites
        * Pinterest
        * Lookbook
        * Polyvore
        * Instagram? Exists
        * Twitter? Exists
    * Set up data base (Firebase?) and collect data
* **Front-End:**
    * Create a template for the outfit combinations
    * Survey forms for each user to fill out their preferences
* **Dev/Ops or QA:**
    * Find web hosting for staging app
    * Set up testing strategy


###This code base uses these python libraries:

**Basic Requirements**

* [Flask](http://flask.pocoo.org/docs/) Web Framework
* Flask-SQlalchemy
* Flask-WTF
* MySQL-python==1.2.4
* Bootstrap
* [Database]() TBD


###Project Structure

    ├── Procfile
    ├── Procfile.dev
    ├── app.py
    ├── config.py
    ├── error.log
    ├── forms.py
    ├── models.py
    ├── requirements.txt
    ├── static
    │   ├── css
    │   │   ├── boostrap-responsive.css
    │   │   └── bootstrap.css
    │   ├── img
    │   │   ├── glyphicons-halflings-white.png
    │   │   └── glyphicons-halflings.png
    │   └── js
    │       ├── libs
    │       │   ├── bootstrap.min.js
    │       │   ├── jquery.min.js
    │       │   └── modernizr-2.0.6.min.js
    │       ├── plugins.js
    │       └── script.js
    └── templates
        ├── 404.html
        ├── 500.html
        ├── index.html
        ├── login.html
        ├── register.html
        └── template.html

Quick Start
----------

1. Clone the repo

        $ git clone git@github.com:DreamsofPy/Style_for_Engineers.git
        $ cd Style_for_Engineers

2. Initialize and activate a virtualenv:

        $ virtualenv --no-site-packages env
        $ source env/bin/activate

4. Install the dependencies:

        $ pip install -r requirements.txt

5. Run the development server:

        $ python app.py

6. Navigate to [http://localhost:5000](http://localhost:5000)

Learn More
---------

1. [Flask Documentation](http://flask.pocoo.org/docs/)
2. [Flask Extensions](http://flask.pocoo.org/extensions/)
3. [flask boilerplate](https://github.com/DreamsofPy/flask-boilerplate)
