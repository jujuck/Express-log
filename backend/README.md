# MVC Express

## Description

This repository is a simple Express MVC structure from scratch.

## Steps

1. Clone the repo from Github.
2. Run `npm install` or `yarn install`.
3. Create _.env_ from _.env.sample_ file and add your DB parameters. Don't delete the _.sample_ file, it must be kept.

```
DB_HOST=your_db_host
DB_PORT=your_db_port
DB_USER=your_db_user
DB_PASSWORD=your_db_password
DB_NAME=your_db_name
```

4. database.sql_ wis done with a dataset. Import the script in your SQL server. You can do it manually or run _migrate_ script (either using `npm run migrate` or `yarn run migrate`).
5. Start the server in dev mode with `npm run dev` or `yarn run dev`. This will run `index.js` using _nodemon_.
6. Go to `localhost:5000/cars` with your favorite browser.
7. From this starter kit, you will implement your logger.
8. On the route 'POST' and 'PUT', there is already a data validation with joy.

### Windows Users

If you develop on Windows, you should edit you git configuration to change your end of line rules with this command :

`git config --global core.autocrlf true`

## Example

An example (a basic list of items) is provided (you can load the _database.sql_ file in a test database). The accessible URLs are :

- Home page: [GET localhost:5000/](localhost:5000/)
- Cars browse: [GET localhost:5000/cars](localhost:5000/cars)
- Cars read: [GET localhost:5000/cars/:id](localhost:5000/cars/2)
- Cars edit: PUT localhost:5000/cars/:id
- Cars add: POST localhost:5000/cars
- Cars deletion: DELETE localhost:5000/cars/:id

You can find all these routes declared in the file `src/router.js`. You can add your own new routes, controllers and models.
