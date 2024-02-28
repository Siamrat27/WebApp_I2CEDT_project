# i2cedt Final Project Group 46
<p>โปรเจกต์ทำเว็บ เว็บที่เราทำคือเว็บเล่นเกมทายคำศัพท์ง่ายๆ</p>
<p>โปรเจกต์วิชา Introduction to CEDT</p>
<p>ทำ Web Application, Store และ Deploy ที่ AWS EC2</p>

## Project Name: Guess The Words
<p>จะมีคำศัพท์ภาษาอังกฤษขึ้นมา และเราต้องทายคำแปลของคำศัพท์</p>

## How to use
in ubuntu

```
sudo apt update -y && sudo apt upgrade -y
```

we will use nvm to download nodejs (nvm: node version manager)

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.5/install.sh | bash
```

we will use latest lts version  (Note that “lts/hydrogen” is an alias for Node 18 LTS.)

```
nvm install lts/hydrogen
```

go into folder backend and install node modules

```
cd backend
npm install
```

do the same but in folder front end

```
cd frontend
npm install
```

next: set up mongodb and change the variable MONGO_URL in /backend/.env

next: set up EC2 instance and change the variable BACKEND_URL in /frontend/scripts/config.js

run this command in backend and frontend folder

```
npm start
```

we define this start script in package.json

`npm start` is the same meaning as `node server.js`

### in backend
- express
- cors
- mongoose
- dotenv

### in frontend
- express
