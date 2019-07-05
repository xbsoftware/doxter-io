Doxter
======

### How to start

You need to have a server with [Docker](https://www.docker.com/) installed

- copy docker-compose.yml from this repo to some folder on the server
- edit docker-compose.yml
	- set EmailService_* values to reflect your email server settings ( if you don't have one, you can can use something like [mailgun](https://www.mailgun.com/) which has a free tier )
	- set RootUser_Login to your email
	- set RootUser_Password to the desired password
- run ```docker-compose up -D``` to start the service

Service will be available at http://localhost:80

### Using with HTTPS

While service works with http only, you can user reverse proxy ( nginx ) to enforce https usage

### Limitations

Image contain fully functional version of service. Still, it is a trial version, which will expire in June 2020. At that point you will need to by a license to continue using the service.

