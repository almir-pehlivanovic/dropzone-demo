### Dropzone Demo project

#####Short project description
The goal of this demo project is a short simulation of CRUD (Create, Read, Update, Delete) operations, as well as file management (adding and deleting from the server). The simulation form is based on drag and drop logic with files and additional fields in the form (title, body, etc.).

The Drag and Drop container allows a maximum of 10 images up to 2MB in .jpg and .jpeg formats.

###Requirements
- PHP version 7.3+
- Composer v2[Composer v2](https://getcomposer.org/download/ "Composer v2")

###Installation
Clone GitHub repo locally

	 git clone https://github.com/almir-pehlivanovic/dropzone-demo.git

Open the folder

	cd dropzone-demo

Install Composer Dependencies

	composer install

Install NPM Dependencies

	npm install

Create a copy of .env file

	cp .env.example .env

Generate an app encryption key

	php artisan key:generate

 Create an empty database for application

 	DB_NAME = dropdown_demo

In the .env file, add database information to allow Laravel to connect to the database

	DB_CONNECTION=mysql
	DB_HOST=127.0.0.1
	DB_PORT=3306
	DB_DATABASE=dropdown_demo
	DB_USERNAME=root
	DB_PASSWORD=

Migrate the database

	php artisan migrate

Seed the database

	php artisan db:seed

Link the storage folder

	php artisan storage:link

Start Laravel application on local development server

	php artisan serve

Open the project in the broweser

	127.0.0.1:8000/
