# udacity-linux-project
IP Address: 35.182.152.20
URL: http://ec2-35-182-152-20.ca-central-1.compute.amazonaws.com

The final project for the linux server configuration course of the Udacity Full Stack Nanodegree.
For this project I configured a Ubuntu 16.04.4 server on Amazon Web Services (AWS), and installed the
catalog final project, of the Back End course, for the Udacity Full Stack Nanodegree.

The following sofware was used:
* Ubuntu 16.04.4
* apache2
* libapache2-mod-wsgi python-dev
* postgresql
* finger
* git
* python-flask
* python-httplib2
* python-flask-sqlalchemy
* python-oauth2client

Configurations made:
* Configured the settings in `catalog.conf` file to direct apache to the project files and directories in `/var/www/catalog/`.
* Changed the `application.py` file in the catalog directory to `__init__.py`.
* Created a `catalog.wsgi` file importing the app from `__init__.py`.
* Created a sudo user for the project reviewer to be able to review the project.
* Created a user with permissions for the database required to run the application.
* Created the database using the `models.py` file.
* Changed OAuth restrictions on Google Cloud Console to the required restrictions.
* Configured and enabled ufw to allow communcation on ports 80/tcp, 123/udp, 2200/tcp.
* Disabled ufw access on port 22.
* Changed references in `__init__.py` and `models.py` to reflect new locations on server.

When stuck on a few issues I used the following repository to help me get in the right direction:
https://github.com/hicham-alaoui/ha-linux-server-config




