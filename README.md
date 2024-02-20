
平平创建的组件库

1、创建一个能适用于不同前端框架的组件库
- 原生Js，Ts
- Vue Cli的Library模式/React的Library模式
  
2、新建项目代码并推送到npm
- 注册npm
- npm run build（npm publish前并不需要先build）
- npm login
  vscode终端中登录npm   可能会遇到Public registration is not allowed(不允许公开注册)的问题：解             法：npm下载源要换成 https://registry.npmjs.org/
  查看下载源：npm config get registry
  设置下载源：npm config set registry 下载源  https://registry.npmmirror.com
  查看不同镜像源：nrm  ls

  新建.npmrc文件后，设置【registry=https://registry.npmjs.org/】，这样就不用来回切换下载源
  
3、npm publish （一定要先npm login）
- 修改版本号   
- package.json中private属性!=true   
- 再次推送时需要修改version

4、npm unpublish chp-element@0.1.4 --force   删掉上传的包

5、npm库中即可看到上传的组件库
