## Simple crud apis for simple CRM.
CRM is using express router and mongodb for database operations. To update or get configuration values refer .env file in the root location.

### Directory Structure
- controllers/
   - clientsController.js
   - leadsController.js
   - salesController.js
- models/
   - client.js
   - lead.js
   - sale.js
- routes/
   - clientRouter.js
   - index.js
   - leadRouter.js
   - saleRouter.js
- views/
   - public/
   - src/
      - components/
         - Client.js
		 - Sale.js
		 - Lead.js
      - App.js
      - App.css
      - index.js
      - index.css
   - package.json
- app.js
- package.json
- README.md
- .env


### .env file
```
MONGO_DB_URL=mongodb://<hostname>:<mongodb-port-number>/<dbname>
SERVER_PORT=<server-port-number>
```

### New route
After creating new route file include it into routes/index.js

### Run the app
To run the applcation make sure you have **nodejs** and **mongodb** installed locally.
Run `npm install` to install all the dependencies.
Run `npm run dev` to run the application

### Mongodb database
After installing mongodb on your local machine or VM or docker create a database in it.
Run command `mongo` in the terminal. Then run `use <dbname>` where dbname is the name of your databse.
Update the databse name in the .env file **MONGO_DB_URL** variable.

## Mongo db connection error on windows
1) mkdir c:\data
2) cd data
3) Run command `mongod -dbpath .`