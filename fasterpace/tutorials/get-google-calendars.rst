Get Google Calendars Website
================================================

By `Jack Henderson`_


In this tutorial, you’ll create a website to Get Google Calendars.

.. contents:: In this article:
  :local:
  :depth: 1

Prerequisites
-------------
Before you start, make sure...

.. note:: For additional information...

Create MVC 6 Website
------------------------------

Start Visual Studio 2015 and select **File|New|Project**.

.. image:: get-google-calendars/_static/0100-CreateProject.png
.. image:: get-google-calendars/_static/0110.png
.. image:: get-google-calendars/_static/0120.png

Entity Framework 7, ASP.NET 5, MVC 6 (google signin)
. Calendar Google to get Mema appointments and create a Travel log for Taxes.
1. Create web app http://docs.asp.net/en/latest/security/authentication/sociallogins.html
. for secrets: https://readthedocs.com/projects/aspnet-aspnet/downloads/pdf/latest/ search for secrets.json
. look for tutorial that gives config switching for dev/test/live settings

Add third party login

https://docs.asp.net/en/latest/security/authentication/sociallogins.html

Create Facebook app
^^^^^^^^^^^^^^^^^^^

google: create app FPTest with url https://localhost:44300/
Use whatever url port you can get!

.. image:: get-google-calendars/_static/0200.png

.. image:: get-google-calendars/_static/0210.png

.. image:: get-google-calendars/_static/0220.png


Facebook
https://developers.facebook.com/apps/

.. image:: get-google-calendars/_static/0230.png

.. image:: get-google-calendars/_static/0240.png

.. image:: get-google-calendars/_static/0250.png

.. image:: get-google-calendars/_static/0260.png


http://www.fasterpace.com/images/FPLogo2.jpgfb: create app FPTest with url https://localhost:44300/
Enable SSL with 44300 for url
http://localhost:44300/

.. image:: get-google-calendars/_static/0270.png


Add nugget package:
Microsoft.AspNet.Authentication.Facebook
Microsoft.AspNet.Authentication.Google


