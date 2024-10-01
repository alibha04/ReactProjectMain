### Create React project

```
npx create-react-app <project name>
cd <project name>
```

### install axios

```bash
npm install axios
```

### Setup a temporary database

- Install the json-server package to hold a json file as the temp db.
- Install it locally and globally both
    ```bash
    npm install -g json-server
    npm install json-server
    ```

- Create a db.json file in the root location of the project and add sample data in it
    ```json
    {
    "persons": [
        { "id": 1, "name": "Alice", "age": 25 },
        { "id": 2, "name": "Bob", "age": 30 }
    ]
    }
    ```

- Run the db
    ```bash
    json-server --watch db.json --port 3001
    ```
### Run the application

- Run the db in one tab first and then the application in another tab(by splitting the terminal)
- After running the db by using " json-server --watch db.json --port 3001",split the terminal
- in the second terminal run the server by using "npm start"
- make the server and db public so that they can access each other

## How to solve the "failed to fatch" error
- if you get an error like this  "failed to fatch" then go to your "PersonList.js" and change the "API-URL" with the URL of your react app(which opens when you run the program)
- After that copy the URL of your react app and paste it on "API-URL" of "PersonList.js"
- then make the port number to "3001"
- then add "persons" after "gitpod.io/"
- then refresh the react app page to see the output

### The output looks something like this

- **Entry page**
![alt text](image.png)

- **Edit page**
![alt text](image-1.png)
