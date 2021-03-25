# node-simple-recipe-api

Simple node Recipe API made with the help of article : [Writing ES6 in NodeJS using Babel](https://medium.com/@abs4real16.ma/writing-es6-in-nodejs-using-babel-10731b8032fc)

# Route List

## Main GET endpoint

- http://localhost:3000/api/v1/

Response body should be :

    {
     "Recipe API": "Healthy"
    }

## Recipe GET endpoint 


- http://localhost:3000/api/v1/recipe

Displays all existing recipes

 Response body should be : 
    
    {
     "count": 1,
     "message": "List of all Recipe",
     "Recipe": [
         {
             "id": 1,
             "name": "gbegiri",
             "description": "It is a yoruba local soup, it is sweet on amala",
             "addedAt": "2020-02-21T00:32:15.254Z"
         }
     ]
    }

## Recipe POST endpoint 

- http://localhost:3000/api/v1/recipe

Adds a recipe

Request body example : 
    
    {
     "name": "Moi-Moi",
     "description": "Moi-Moi is very sweet, made from bean flour"
    }

Response body should be :

    {
     "message": "A new recipe has been added",
     "data": {
        "id": 2
     }
    } 


## 404 route

- http://localhost:3000/{slug}

API Endpoint not found

Response body should be :

    {
     "error": true,
     "message": "Route Not found"
    }



## Local Setup

Considering you already downloaded the code you must follow these steps:

Use the package manager [npm](https://www.npmjs.com/) to install package.json dependencies.

```bash
npm install
```
And finally run the server on your local machine
> make sure you have [node](https://nodejs.org/en/download/) installed on your machine

```
npm start
```
## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

Please make sure to update tests as appropriate.
