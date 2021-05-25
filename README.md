# 初始化配置文件

安装node并在终端运行：

```shell
npm init -y
```

安装ts：`npm i -G typescript`初始化配置

```shell
tsc -init
```

webpack配置文件

```shell
touch webpack.config.js
```

# 完善目录结构

```sh
.
├── package.json 
├── src
│   ├── index.html #html模板
│   ├── index.ts #入口文件
│   ├── modules #模块目录
│   │   ├── Food.ts #食物模块
│   │   ├── GameCtl.ts #游戏控制
│   │   ├── ScorePanel.ts #分数面板
│   │   └── Snake.ts #蛇模块
│   └── style #样式目录
│       └── index.less #样式
├── tsconfig.json
└── webpack.config.js
```

# 安装模块

```bash
npm i -D webpack webpack-cli typescript ts-loader html-webpack-plugin clean-webpack-plugin  webpack-dev-server @babel/core @babel/preset-env babel-loader core-js less less-loader css-loader style-loader postcss postcss-loader postcss-preset-env
```

1. 安装**webpack**

   ```bash
   npm i -D webpack webpack-cli  
   ```

2. 安装**typescript**

   ```bash
   npm i -D typescript ts-loader
   ```

3. 安装**html**

   ```bash
   npm i -D html-webpack-plugin
   ```

4. 安装**clean-webpack-plugin**

   ```bash
   npm i -D clean-webpack-plugin
   ```

5. 安装**webpack-dev-server**

   ```bash
   npm i -D webpack-dev-server
   ```

   修改**package.json**

   ```json
   {
     "name": "snake",
     "version": "1.0.0",
     "description": "贪吃蛇",
     "main": "index.js",
     "scripts": {
       "test": "echo \"Error: no test specified\" && exit 1",
       "build": "webpack",
       "start": "webpack serve --open chrome.app",
       "dev": "webpack serve --open chrome.exe"
     },
     "repository": {
       "type": "git",
       "url": "git+https://github.com/shijinke1990/snake.git"
     },
     "keywords": [],
     "author": "",
     "license": "ISC",
     "bugs": {
       "url": "https://github.com/shijinke1990/snake/issues"
     },
     "homepage": "https://github.com/shijinke1990/snake#readme",
     "devDependencies": {
       "@babel/core": "^7.14.3",
       "@babel/preset-env": "^7.14.2",
       "babel-loader": "^8.2.2",
       "clean-webpack-plugin": "^4.0.0-alpha.0",
       "core-js": "^3.12.1",
       "css-loader": "^5.2.6",
       "html-webpack-plugin": "^5.3.1",
       "less": "^4.1.1",
       "less-loader": "^9.0.0",
       "postcss": "^8.3.0",
       "postcss-loader": "^5.3.0",
       "postcss-preset-env": "^6.7.0",
       "style-loader": "^2.0.0",
       "ts-loader": "^9.2.2",
       "typescript": "^4.2.4",
       "webpack": "^5.37.1",
       "webpack-cli": "^4.7.0",
       "webpack-dev-server": "^3.11.2"
     }
   }
   
   ```

6. 安装**bable**

   ```bash
   npm i @babel/core @babel/preset-env babel-loader core-js -D
   ```

7. 安装**less**及相关

   ```bash
   npm i -D less less-loader css-loader style-loader 
   ```

   ```bash
   npm i -D postcss postcss-loader postcss-preset-env
   ```

#  package.json

```json
{
  "name": "snake",
  "version": "1.0.0",
  "description": "贪吃蛇",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "repository": {
    "type": "git",
    "url": "git+https://github.com/shijinke1990/snake.git"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "bugs": {
    "url": "https://github.com/shijinke1990/snake/issues"
  },
  "homepage": "https://github.com/shijinke1990/snake#readme"
}

```

