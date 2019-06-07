### 说明

### 查看版本信息
```aidl
node -v
```

### 运行nodejs
- js文件: index.js
```aidl
console.log("Hello World");
```
- nodejs 运行js
```aidl
node index.js
```


### 交互模式
```aidl
node

console.log('hello');

```

### Http server启动
- 新建 server.js
- 运行 node server.js
```aidl
var http = require('http');

http.createServer(function (request, response) {

    // 发送 HTTP 头部 
    // HTTP 状态值: 200 : OK
    // 内容类型: text/plain
    response.writeHead(200, {'Content-Type': 'text/plain'});

    // 发送响应数据 "Hello World"
    response.end('Hello World\n');
}).listen(8888);

// 终端打印如下信息
console.log('Server running at http://127.0.0.1:8888/');
```