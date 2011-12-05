django-lines
===
Show the lines of code in a django project, excluding django's automatically created stuff. A simple script to get the most basic metric on your project.

INSTALLATION
------------
    $ git clone git://github.com/stevematney/django-lines.git
	$ cd django-lines 
	$ mv django-lines your/preferred/path/django-lines
	$ django-lines --help

REMOVAL
--------------------------------------
    $ cd /path/to/django-lines
    $ rm django-lines

USAGE
-----
Usage: django-lines [OPTIONS] [path]

COMMANDS:
    --help, -h               
        Show this message

    -p
        Show only production code (excluding tests).

    -t
        Show only test code

QUICK EXAMPLE
-------------
	$ django-lines
     20 .//fake_app/models.py
     95 .//fake_app/tests.py
      8 .//fake_app/urls.py
     10 .//fake_app/views.py
    102 .//settings.py
     24 .//templates/base.html
      1 .//templates/index.html
     30 .//templates/login.html
     21 .//urls.py
      4 .//views.py
    315 total
    
    $ django-lines -p
     20 .//fake_app/models.py
      8 .//fake_app/urls.py
     10 .//fake_app/views.py
    102 .//settings.py
     24 .//templates/base.html
      1 .//templates/index.html
     30 .//templates/login.html
     21 .//urls.py
      4 .//views.py
    220 total

    $ django-lines -t
     95 .//fake_app/tests.py

