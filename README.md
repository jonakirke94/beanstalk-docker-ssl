﻿# SingleInstance Docker enviorement with SSL in AWS Beanstalk.

Single instance docker enviorement with SSL on AWS Beanstalk.

The following ENV variables should be present in .ebextensions/ssl.config:

DOMAIN_EMAIL
DOMAIN_URL

The domain url you wish to retrieve a certificate for should have a DNS record that points to the server this application is running on. Certbot will create
an ACME-challenge on this webserver and verify it.
