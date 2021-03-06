Rouncube Plugin rcguard
=======================

Introduction
----------------------------------------
This plugin logs failed login attempts and requires users to go through
a reCAPTCHA verification process when the number of failed attempts go
too high. This provides protection against automated attacks.

Failed attempts are logged by IP and stored within MySQL. IPs are also
released after a certain amount of time.

The original author of this plugin is Denny Lin (https://github.com/dennylin93). 
I forked it some years ago to add reCAPTCHA v2.0, add the larry skin 
and because the project issues were taking too long to be answered.
Also, the original project is not updated since 2015 and many things 
have changed in the meantime in Roundcube's code.

Installation
----------------------------------------
Place this directory under plugins/, and enable rcguard within the main
configuration file.

Copy config.inc.php.dist to config.inc.php and modify as necessary.

Use the files within SQL/ to create the database layout required for
rcguard. The table should be created in the database used by Roundcube.

Please note that this plugin requires reCAPTCHA API keys to work properly.
They can be obtained from http://www.google.com/recaptcha.

Customizing reCAPTCHA
----------------------------------------
Different themes and translations are available. If none of them fit
your needs, create a custom one.

Documentation about the reCAPTCHA:
https://developers.google.com/recaptcha/intro

Supported databases
----------------------------------------
- MySQL
- PostgreSQL
- SQLite

License
----------------------------------------
This plugin is distributed under the BSD license. Please see rcguard.php
for the complete license.

This plugin also contains a PHP library for reCAPTCHA that is
distributed under its own license. See the file for exact details.

Contact
----------------------------------------

The original author of this plugin is Denny Lin (https://github.com/dennylin93). 
I forked the project some years ago and i'm maintaining it because i need 
it working with the latest version of Roundcube.

Comments and suggestions are welcome (preferentially via issues).

Email: [Diana Soares][email]

[email]: mailto:diana.soares@gmail.com

