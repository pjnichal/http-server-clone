
# HttpServerClone

HttpServerClone is a lightweight npm package that provides a simple clone of Express.js but with a TCP server. It allows you to handle basic routing for TCP requests in a manner similar to how Express.js handles HTTP requests.

**THIS PROJECT IS ONLY FOR LEARNING DO NOT USE THIS PACKAGE AT PRODUCTION**
## Installation Guide

install package using npm

```bash
  npm i http-server-clone
```


## Usage

```javascript
const { httpServerClone } = require("http-server-clone");
const app = httpServerClone();

app.get("/getTest", (req, res) => {
  res.status(200).send("YEAHH");
});
app.get("/getJson", (req, res) => {
  res.status(200).json({ message: "JSON WORKING" });
});

app.listen("8080", () => {
  console.log("Sever Running on 8080");
});
```
Currently Supported Methods : GET, POST, DELETE, PUT, PATCH 

## Github & Linkedin

 - [http-server-clone - Github](https://github.com/pjnichal/http-server-clone)
  - [http-server-clone - NPM](https://www.npmjs.com/package/http-server-clone)
 - [Portfolio](https://pravinnichal.in/)


## Contributing & Usage

Contributions are always welcome!

Make a pull request or raise an issue.


