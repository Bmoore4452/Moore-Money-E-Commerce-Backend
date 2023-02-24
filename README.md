# Moore-Money-E-Commerce-Backend

## Description

This is a project that creates the back end for for an e-Commerce website. It performs all aspects of the CRUD process.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Questions](#questions)

## Installation

First, the user must use the [MySQL2](https://www.npmjs.com/package/mysql2) and [Sequelize](https://www.npmjs.com/package/sequelize) packages to connect your Express.js API to a MySQL database and the [dotenv](https://www.npmjs.com/package/dotenv) package to use environment variables to store sensitive data. In addition, the user will need to have the application installed to test the routes [Insominia](https://insomnia.rest/).

## Usage

The user will first need use the `schema.sql` file in the `db` folder to create your database with MySQL shell commands. Use environment variables to store sensitive data like your MySQL username, password, and database name. Then the user will need to run `npm run seed` to seed data to your database so that you can test your routes. After seeding the data, the user can run this list of test to test the API routes:

### Test Plan:

- seed data on mysql
- npm run seed
- npm run watch

### Run these commands in Insomnia:

---

GET:
`http://localhost:3001/api/products
http://localhost:3001/api/tags
http://localhost:3001/api/categories`

---

GET:
`http://localhost:3001/api/products/1
http://localhost:3001/api/tags/2
http://localhost:3001/api/categories/3`

---

POST:
`http://localhost:3001/api/products/`

```
{
   "product_name": "Basketball",
   "price": 200.00,
   "stock": 3,
   "tagIds": [1, 2, 3, 4]
}
```

`http://localhost:3001/api/categories/`

```
{
   "category_name": "Underwear"
}
```

`http://localhost:3001/api/tags/`

```
{
   "tag_name": "Cool Tag"
}
```

PUT:
`http://localhost:3001/api/products/6`

```
{
   "product_name": "NBA Official Basketball",
   "price": 200.00,
   "stock": 3,
   "tagIds": [1, 2, 3, 4]
}
```

`http://localhost:3001/api/categories/6`

```
{
   "category_name": "Undergarments"
}
```

`http://localhost:3001/api/tags/9`

```
{
   "tag_name": "Super Cool"
}
```

DELETE:
`http://localhost:3001/api/products/1
http://localhost:3001/api/categories/1
http://localhost:3001/api/tags/3`

## Questions

Here is a link to my Github account:
[Bmoore4452](https://github.com/Bmoore4452)

Please feel free to contact me at r.moore803@gmail.com with instructions on how to reach me with additional questions
