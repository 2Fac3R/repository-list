# Repository List
## Description

This project was crafted as part of a Laravel course on platzi.com. It showcases a repository list, with the primary focus being on following the Test-Driven Development (TDD) methodology. The approach involves initially creating tests, followed by developing the corresponding functionalities, and finally, refining the codebase through refactoring.

Stack:

* PHP (7.3) + Laravel (8)
* Testing Framework: PHPUnit
* HTML (Blade Templates) + CSS (TailwindCSS Framework)

## One-Time Setup

1. Copy the `.env.example` file to `.env`:
   ```bash
   cp .env.example .env
   ```
2. Update `.env` with your desired configuration (`DB_HOST=db`, etc.).
3. Generate the application key:
   ```bash
   docker compose exec app php artisan key:generate
   ```
4. Run migrations and seed the database:
   ```bash
   docker compose exec app php artisan migrate --seed
   ```


## Usage

Log in or create a new user, user profile settings...

    http://127.0.0.1:8000/dashboard
    http://127.0.0.1:8000/register
    http://127.0.0.1:8000/login
    http://127.0.0.1:8000/user/profile
    
You can access to the following resources routes

    http://127.0.0.1:8000/repositories

Create a new repository

    http://127.0.0.1:8000/repositories/create

Get a repository by id

    http://127.0.0.1:8000/repositories/<id>

Edit a repository by id
 
    http://127.0.0.1:8000/repositories/<id>/edit

## Running tests

There are 18 test divided in unit and feature tests

    Unit/Models/UserTest.php
    Unit/Models/RepositoryTest.php
    Feature/Http/Controller/PageControllerTest.php
    Feature/Http/Controller/RepositoryControllerTest.php

Run Test

    php artisan test
    

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Any feedback is appreciated.
