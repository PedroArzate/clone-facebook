# clone-facebook
Clone Facebook Test

# ![Laravel Example App](https://user-images.githubusercontent.com/22407783/225290976-129dcc1f-f91b-404b-b05a-280719a3be82.png)



> ### Example developed in Laravel 9.0 containing a real example of a Facebook clone API.
This repo is a technical test!

----------

# Getting started

## Installation

Please check the official laravel installation guide for server requirements before you start. [Official Documentation](https://laravel.com/docs/9.x/installation) 

Clone the repository

    git clone git@github.com:PedroArzate/clone-facebook.git

Switch to the repo folder

    cd clone-facebook

Install all the dependencies using composer

    composer install

Copy the example env file and make the required configuration changes in the .env file

    cp .env.example .env

Run the database migrations (**Set the database connection in .env before migrating**)

    php artisan migrate

Start the local development server

    php artisan serve

You can now access the server at http://localhost:8000/api/v1

**TL;DR command list**

    git clone git@github.com:PedroArzate/clone-facebook.git
    cd clone-facebook
    composer install
    cp .env.example .env
    
**Make sure you set the correct database connection information before running the migrations** [Environment variables](#environment-variables)

    php artisan migrate
    php artisan serve

## Postman Test

Testing via postman can be done using a Postman Collection. This contains the web services for Posts and Groups.

> [Clone-Facebook.postman_collection.zip](https://github.com/PedroArzate/clone-facebook/files/10979350/Clone-Facebook.postman_collection.zip)


----------

# Code overview

## Folders

- `app` - Contains all the Eloquent models
- `app/Http/Controllers` - Contains all the api controllers
- `app/Http/Requests` - Contains all the api form requests
- `app/Http/Controllers/PostsController` - Contains the files implementing the posts methods
- `app/Http/Controllers/GroupsController` - Contains the files implementing the groups methods
- `config` - Contains all the application configuration files
- `database/factories` - Contains the model factory for all the models
- `database/migrations` - Contains all the database migrations
- `database/seeds` - Contains the database seeder
- `routes` - Contains all the api routes defined in api.php file

## Environment variables

- `.env` - Environment variables can be set in this file

***Note*** : You can quickly set the database information and other variables in this file and have the application fully working.
