# nodejs
[nodejs](https://nodejs.org/en/ "nodejs")

###更新命令
- npm update –g 在windows下不能更新成功 
- Not compatible with your operating system or architecture: n@2.1.4
  - 这个package的源码，它是把node的安装路径写死了的，非默认安装都会提示没有安装node

1. [nvm](https://github.com/creationix/nvm "bash")
2. [nvm-windows](https://github.com/coreybutler/nvm-windows "nvm-windows")
3. 

###查看版本
- node -v
- 

###Hello World
```
  const http = require('http');
  
  const hostname = '127.0.0.1';
  const port = 3000;
  
  const server = http.createServer((req, res) => {
    res.statusCode = 200;
    res.setHeader('Content-Type', 'text/plain');
    res.end('Hello World\n');
  });
  
  server.listen(port, hostname, () => {
    console.log(`Server running at http://${hostname}:${port}/`);
  });
  ```
  
  To run the server, put the code into a file called example.js and execute it with Node.js:

```
  $ node example.js
  Server running at http://127.0.0.1:3000/
```

All of the examples in the documentation can be run similarly.
  
  
  
