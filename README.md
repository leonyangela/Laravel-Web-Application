#  Laravel Ecommerce CRUD Example

<p>Example Laravel codebase containing real world examples (CRUD, auth (admin or user), database and more) that adheres to the RealWorld spec.</p>
<p>This web app is made using laravel v5.5.</p>

## Getting Started
<p>These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.</p>

### Prerequisites
What things you need to install the software and how to install them:
```
1. Server, I use XAMPP(Apache (Server) and MySQL (Database))
2. IDE
3. Browser
4. Composer 
5. Laravel Installed
```

## Installation
Please check the official laravel installation guide for server requirements before you start. <a href="https://laravel.com/docs/5.5/installation">Official Documentation</a>

Clone the repo
```
git clone https://github.com/leonyangela/laravel-ecommerce-crud-example.git
```

Switch to the repo folder
```
cd laravel-ecommerce-crud-example
```

Open ".env.example"
```
Change the Database Config depends on your setup

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=YOUR DATABASE NAME
DB_USERNAME=YOUR USERNAME DATABASE
DB_PASSWORD=YOUR PASSWORD DATABASE 
```

Generate a new application key
```
php artisan key:generate
```

Run the database migrations (Set the database connection in .env before migrating)
```
php artisan migrate
```

Start the local development server
```
php artisan serve
```

You can now access the server at http://localhost:8000

### TL;DR command list
```
git clone https://github.com/leonyangela/laravel-ecommerce-crud-example.git
cd laravel-ecommerce-crud-example
composer install
php artisan key:generate
```

Make sure you set the correct database connection(from .env files) information before running the migrations.
```
php artisan migrate
php artisan serve
```

## Database seeding
Populate the database with seed data with relationships which includes users, product, and brand. This can help you to quickly start testing the api or couple a frontend and start using it with ready content.

Open the Seeder and set the property values as per your requirement
```
database/seeds/DatabaseSeeder.php
```

Run the database seeder and you're done
```
php artisan db:seed DatabaseSeeder
```

<em>Note</em> : It's recommended to have a clean database before seeding. You can refresh your migrations at any point to clean the database by running the following command

```
php artisan migrate:refresh
```

## Please pay attention to this Note
* <p style="color: red"><em>Note</em>: If you want to access as admin, just change the database from:</p>
```
admin: 0
```
to
```
admin: 1
```
* Please do 
``` 
php artisan migrate 
```
before
```
php artisan db:seed
```
* Make sure you set the correct database connection(from .env files) information before running the migrations.

## Built With
* Laravel v5.5
* Bootstrap v4.1.3 

If you have any suggestion or found some debug, feel free to contact me.
