# big-ideas
The main repsoitory for the language learning tool codenamed Zeta Beta.

How to setup your local environment
	
	1. Get the repository via:
		Option 1. Using git bash/terminal to clone the repository
			$ git clone https://github.com/ZetaBetaLanguages/big-ideas.git
		
		Option 2. Download the zip file using your web-browser.
			https://github.com/ZetaBetaLanguages/big-ideas/archive/master.zip
	
	2. Use composer to install dependencies
		Option 1: Composer is not installed globally

			$ cd laravel
			$ curl -s https://getcomposer.org/installer | php
			$ php composer.phar install

		Option 2: Composer is installed globally

			$ cd laravel
			$ composer install

	3. Configure your database.
			Make sure your mysql server is configured and running properly. Create an empty database which zetabeta will use.
	
	4. Configure your environment.
			Edit your .env files located in the laravel root folder so it matches the credentials needed to access your own local database
	
	5. Populate database
			Run these commands to create and populate Users table:

			$ php artisan migrate
			$ php artisan db:seed
