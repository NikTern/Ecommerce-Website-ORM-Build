# Ecommerce Backend System!
Ecommerce site backend built using Express, Sequelise, MySQL.

## Description

This project is a backend server for an e-commerce website where customers can browse products by categories and tags built using Node.js and Express.js, using Sequelize as the ORM for working with a MySQL database.

Customers can browse products by categories and tags, and the server provides REST API routes to perform CRUD operations on categories, tags, and products.

## Installation

The project can be accessed at: https://github.com/NikTern/Ecommerce-Website-ORM-Build

Installation steps:
1. Install Node.js and MySQL if not already installed on your machine.
2. Install the dependencies with 'npm install' in the command line
3. Modify the password field in the .env file with your own MySQL database name, user, and password.
4. Create a MySQL database using the schema.sql file provided in the repository.
5. Seed the database with 'npm run seeds'
6. Run the application with 'node server.js'

## Usage

Walkthrough Video: https://drive.google.com/file/d/1jPTZCZNCp-1P78ST5nk4hmWOqKV_5QVC/view?usp=sharing

This application permits the user to perform various CRUD operations, which they can do by sending the following requests to the appropriate url:

GET requests: 

    a. GET /api/categories: This request retrieves all categories from the database and their associated products.

    b. GET /api/categories/:id: This request retrieves a specific category and its associated products, using the ID parameter to identify the category.

    c. GET /api/products: This request retrieves all products from the database and their associated categories and tags.

    d. GET /api/products/:id: This request retrieves a specific product and its associated category and tags, using the ID parameter to identify the product.

    e. GET /api/tags: This request retrieves all tags from the database and their associated products.

    f. GET /api/tags/:id: This request retrieves a specific tag and its associated products, using the ID parameter to identify the tag.

POST requests:

    a. POST /api/categories: This request creates a new category in the database.

    b. POST /api/products: This request creates a new product in the database, along with any associated tags.

    c. POST /api/tags: This request creates a new tag in the database.

PUT requests:

    a. PUT /api/categories/:id: This request updates a specific category in the database, using the ID parameter to identify the category.

    b. PUT /api/products/:id: This request updates a specific product in the database, along with any associated tags, using the ID parameter to identify the product.

    c. PUT /api/tags/:id: This request updates a specific tag in the database, using the ID parameter to identify the tag.

DELETE requests:

    a. DELETE /api/categories/:id: This request deletes a specific category from the database, along with any associated products, using the ID parameter to identify the category.

    b. DELETE /api/products/:id: This request deletes a specific product from the database, using the ID parameter to identify the product.

    c. DELETE /api/tags/:id: This request deletes a specific tag from the database, along with any associated products, using the ID parameter to identify the tag.


## License

MIT License

Copyright (c) [2022] [NikolasTernezis]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.