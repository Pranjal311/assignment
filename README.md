 backend code in Node.js using Express and Javascript.

## install packages
1. npm install

### to start project locally on localhost:3000
npm run start or NODE_ENV=local node ./src/run.js

### run build on server ###
* NODE_ENV=development pm2 start ./src/run.js --name dev

### localhost URL ###
* http://localhost:3000/


### configure db authentication ###
configure mongodb user/passwor on env file.

db.createUser(
   {
     user: "assignment",
     pwd: "sensehawk",
     "roles" : [ 
        {
            "role" : "readWrite",
            "db" : "adminRcc"
        }
    ]
   }
)