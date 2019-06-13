# electron-demo
### 搭建
- 创建一个新的空文件，执行npm init创建package.json文件，其中的 main 字段所表示的脚本为应用的启动脚本，它将会在主进程中执行。
```markdown
{
  "name": "your-app",
  "version": "0.1.0",
  "main": "main.js"
}
```
注：如果 main 字段没有在 package.json 中出现，那么 Electron 将会尝试加载 index.js 文件（就像 Node.js 自身那样）。 如果你实际开发的是一个简单的 Node 应用，那么你需要添加一个 start 脚本来指引 node 去执行当前的 package：
```markdown
{
  "name": "your-app",
  "version": "0.1.0",
  "main": "main.js",
  "scripts": {
    "start": "node ."
  }
}
把这个 Node 应用转换成一个 Electron 应用也是非常简单的，我们只不过是把 node 运行时替换成了 electron 运行时
{
  "name": "your-app",
  "version": "0.1.0",
  "main": "main.js",
  "scripts": {
    "start": "electron ."
  }
}

```
- 安装electron
```markdown
npm install --save-dev electron
```

- 创建main.js 和 index.html文件

### 执行
- npm install
- npm start