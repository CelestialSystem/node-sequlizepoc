1. npm i express-generator -g
2. express node-sequelize --views=ejs (This will create express js project with ejs view)
3. cd node-sequelize && npm i
4. Now, code .
   Folder structure will look like:-
   > bin
   > node_modules
   > public
   > routes
   > views
   > app.js
   > package-lock.json
   > package.json
5. sudo npm i -g sequelize-cli
6. npm i -S sequelize
7. npm i -S pg pg-hstore
8. touch .sequelizerc (initialize sequelize configuration, this file tells sequel initinialztns to generate config, models, seeders, migrations to specific directories)

9. sequelize init
10. npm i -g sequelize-cli (You can install the sequelize-cli package in your project locally by using -D (equivalent to using --save-dev) instead of the -g (--global) flag)
11. npm i --save sequelize pg pg-hstore
12. sequelize init
13. sequelize model:create --name Todo --attributes title:string
14. sequelize model:create --name TodoItem --attributes content:string,complete:boolean
NOTE: defined the relationship between a Todo and it's TodoItems in the Todo.associate class method. The as: 'todoItems' means that every time we query for a todo and include it's todo items, they'll be included under the key todoItems instead of TodoItems (Sequelize defaults to using the pluralized model name)

15. sequelize db:migrate