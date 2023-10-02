# Welcome to Flight Service

## Project Setup
- clone the proeject on your local
- Execute `npm install` on the same path as of your root directory of the downloaded project
- Create a `.env` file in the root directory and add the following enviorment variable
    - `PORT=3000`
- Inside the `src/config` folder create a new file `config.json` and then add the following piee of json


'''
{
  "development": {
    "username": "<YOUR_DB_NAME>",
    "password": "<YOUR_DB_PASSWORD>",
    "database": "Flight_Search_DB_DEV",
    "host": "127.0.0.1",
    "dialect": "mysql"
  }
}

'''

- Once you've added your db config as listed above, go to the src folder from your terminal and execute `npx sequelize db:create`

```

## DB Design
  - Airplane Table
  - Flight 
  - Airport
  - City

  - A flight belongs to an airplane but one airplane can be used in multiple flights
  - A city has many airports but one airport belongs to a city
  - One airport can have many flights, but a flight belongs to one airport

 