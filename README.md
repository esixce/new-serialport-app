HOW THIS WAS CREATED:

mkdir new-serialport-app
cd new-serialport-app
npm init -y
npm install electron electron-builder --save-dev
npm install typescript @types/node --save-dev
npx tsc --init
npm install serialport @types/serialport --save
touch main.ts

create file:
- main.ts
- index.html
- electron.js

adjust package.json
"main": "electron.js"
"scripts": {
  "start": "electron .",
  "build": "electron-builder"
},

npm start
npm run build