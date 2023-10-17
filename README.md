**_Backend social network- A private social network using nodeJS, express, MySQL & Sequelize_**

**Main branch - Commit #1**

# Description

- This api aims to test multiple SPA.

# Main goals

- This API aims to test frontend applications. :construction:
- The backend is made with NodeJS, Express with MySQL database & Sequelize as ORM.

# Change done

- Create unique repo backend.

# Before to run this server

- :warning: In a terminal, create your own MaraiDB SQL database, named `groupomania` by default with `root` user & `azerty` password.
- In the root of the `/backend` folder, rename the folder called `/images.example` to `/images`.
- Rename `.env.example` into `.env`.
- In a terminal with MySQL, insert this query:

```
CREATE DATABASE groupomania;
```

- In the .env file, insert your parameters :

```
DB_NAME = INSERT DATABASE NAME
DB_USER = INSERT DATABASE USER
DB_USER_PASSWORD = INSERT DATABASE USER PASSWORD
DB_HOST = INSERT DATABASE HOST
DB_DIALECT = mysql
DB_PORT = 3306
APP_PORT = 3001

USER_CRYPTOJS_KEY = INSERT RADOM ASCII CHARACTER
SECRET_TOKEN = INSERT RANDOM ASCII CHARACTER
NODE_ENV = development
```

- In the .env frontend file, insert your parameters:

- :warning: frontend api port value must be equal to APP_PORT one.

# How to run this application

- Open terminal in both frontend and backend repos, then run the following commands :

- Install depedencies :

```
npm install
```

- Launch server :

```
npm start
```

- :warning: In order to prevent from port collisions, the data base port value is 3306 by default.

# How to create an admin user with root privileges :crown:

- In the dabase named `groupomania` by default insert this query with the desired user_id :

```
UPDATE `users` SET `admin` = '1' WHERE `user_id` = '1';
```
