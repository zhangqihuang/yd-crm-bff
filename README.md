BFF项目启动前置条件：

一. 主工程安装npm包和启动服务  
npm install  
npm install -g typescript  
npm install -g ts-node  
npm install -g ts-node-dev  

二. mock-data是一个独立的服务，需要单独安装npm包和启动服务  
cd mock-data  
npm install  
npm install -g express  
node app.js  

三. 测试：  
1. 浏览器访问 http://localhost:4000/ （mock接口）  
2. 浏览器访问 http://localhost:3000/api/test （BFF接口）

四. 添加新接口：  
1. controller/ApiController.ts 增加新接口  
2. 如果需要添加新的controller，需要在ioc/loader.ts中import  