# ts-node-express

this set up for prepare node-express to use typescript incorparate

## #setup nodejs + express

-select folder that want to place the project
-use npm init -y to install package.json
-use npm i express dotenv to install framework and manage sensitive info in env file
-setup app.js or index.js by using express in file
-then run port with node src/index.js or app.js (if you're setup "main" to start in package.json)
-if you're insert "start": in "scripts" and locate that you want to npm run start with you can use it

"You're already done setup nodejs with express"

## #setup typescript

-start install devlopment dependencies for using typescript
-by npm i --dev typescript @types/express $types/node
-and then generate tsconfig.json to manage typescript
-by using npx tsc --init it'll be create tsconfig.json automatically
-open tsconfig explore structure and then fide "outDir" and then uncommented it
-then set "outDir": "./dict" and go to package.json to set "main": "dist/index.js"
-because Typescript code will be complie from src to directory to dict

## #create an express server with a .ts

-change package.json to "main": "dist/index.js for when complie ts to js; you can use "node dict/index.js" to run server
-in tsconfig.json change outDir value to "dict" and rootDir value to "src"

"Done!"

*** if you want to use npm run start instead node dict/index.js every time
