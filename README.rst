Ploomcake PA
============
This is the buildout folder of Ploomcake PA. This buildout extends the Ploomcake buildout (https://github.com/ploomcake/ploomcake_buildout).

What is Ploomcake PA
====================
Ploomcake PA is a distribution of the powerful open source Plone CMS (http://plone.org) that lets you create an out-of-the-box public administration portal.
It automatically includes in your portal a selection of the best third-party open source plugins: xhtml strict templates, styles for partially sighted people, mobile support with responsive theme, easy forms generation support, tabs and slideshows goodies,  and much more.
Before you go on you should know that it is also available a pre packaged unified installer. Go and get it on the official web site (http://www.ploomcake.org).
If you are an expert user (or a developer) you can go on following this guide.

How to install
==============

The first step is to download and install Ploomcake. You can use either the unified installer or follow this https://github.com/ploomcake/ploomcake_buildout).
After the installation, put this folder in the instance directory as "ploomcakepa_config.d". Go to the instance directory and clone this repository from github using::::

    git clone git@github.com:ploomcake/ploomcakepa_buildout.git ploomcakepa_config.d

Pick a buildout
---------------
In the ploomcakepa_config.d folder we have two main buildout files: start_develop.cfg and start_production.cfg
Choose the one to install according to what kind of installation you prefer. If you want to:

    * build a developer environment (with a lot of useful tools, test etc.), pick the start_develop.cfg
    * build a production environment, pick the start_production.cfg

Launch the buildout
-------------------
Copy the buildout file you picked in the parent folder (the instance directory), rename as buildout.cfg and launch::

    bin/buildout

Enjoy!!
-------
Ploomcake PA is installed correctly. You can give a try launching::

    bin/plonectl start

Ploomcake PA will respond to http://localhost:8080.
