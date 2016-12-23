# node-apiblueprint
Node.js下使用API Blueprint格式写API文档的工作环境

[API Blueprint](https://github.com/apiaryio/api-blueprint)使用md文档的格式，快速书写API文档，并且可以通过文档生成便于查看的HTML文档（使用[aglio](https://github.com/danielgtaylor/aglio)），也可以生成测试用的Mock服务器（使用[Drakov](https://github.com/Aconex/drakov)）。

文档书写格式，请查看[API Blueprint](https://github.com/apiaryio/api-blueprint)。一些文档书写例子，请查看https://github.com/apiaryio/api-blueprint/tree/master/examples

## 安装
需要[Node.js](https://nodejs.org)环境
````
$ git clone https://github.com/ihahoo/node-apiblueprint.git
$ npm install
````

## 运行文档转换html服务
通过`src/index.md`来写文档，运行下面的命令，可以以网页形式时时查看文档。
````
$ npm run doc
````
然后通过浏览器打开`http://localhost:3000/`即可查看文档，修改文档的同时可以自动刷新显示。

## 运行API测试服务器（mock）
可以按照API Blueprint的文档格式，自动生成测试api的数据。这样描述好API文档后，前端即可进行一些调用测试。
执行以下命令：
````
$ npm run mock
````
然后通过`http://localhost:3001/`测试接口，在本例子中，可以通过GET http://localhost:3001/test 查看测试的接口样例。

## 生成HTML文档
````
$ npm run build
````
通过此命令，可将文档转换为html并保存到`build`目录下，即可将文档提交给其它开发人员查阅。

## 清理build文件夹
````
$ npm run clean
````
