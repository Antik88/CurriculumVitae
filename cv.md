# Anton Sheinikov
![asd](./img/happyBirthday.jpg)<br>

### Links:
[GitHub](https://github.com/Antik88) / [Telegram](https://t.me/Ant1k1) 
/ [Gmail](mailto:ant1kow22@gamil.com)

# About me
I am a second-year computer science student.
Live in Belarus.
Now I want to develop in the direction of web-development,
to study both front-end and back-end. 
I have not worked or had an internship anywhere, but I have my own projects which I implement little by little to acquire enough skills. 
Writing code with Neovim. Love Gruvbox.

## My stack of technologies 
 - C# 
 - JS
 - React (MUI)
 - Node.js (Sequelize, Express)
 - SQL (PostgreSql, SQLite, MS SQL Server)
 - HTML/CSS
 - Python (site parsing)

## My projects
 - [Weather:](https://github.com/Antik88/weather.git)
React application that shows the weather forecast using an open API

 - [ParserTgBot:](https://github.com/Antik88/AnimeBot.git)
Bot for telegram which parses the site gives a random good anime series, with screenshots 

 - [ShareOnline:](https://github.com/Antik88/ShareOnline.git)
A place where people can rent and lease things, for short-term use

## Code example
User API _registration with jwt token_
```
import { $authHost, $host } from "./index";
import jwt_decode from "jwt-decode";

export const registration = async (email, password) =>{
    const {data} = await $host.post("api/user/registration", {email, password, role: 'USER'})
    localStorage.setItem('token', data.token) 
    return jwt_decode(data.token)
}
```
