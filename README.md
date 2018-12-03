# imooc-vue

- 新建一个vue项目

- 安装mongodb，将resource下dumall-goods,dumall-users导入数据库

  mongoimport -d imooc -c users(goods)  --file FILEPATH

- 修改config/index.js 

  ```
  proxyTable: {
        '/goods': {
          target: 'http://localhost:3000'
        },
        '/goods/*': {
          target: 'http://localhost:3000'
        },
        '/users/*': {
          target: 'http://localhost:3000'
        }
      },
  ```

- 安装express-generator 

  npm i -g express-generator

  创建后端服务server	输入命令 express server	覆盖server下的文件

- 覆盖src代码

- 安装下依赖 npm i 

- 运行node.js后端代码 node ./server/bin/www

- 运行前端代码 npm start