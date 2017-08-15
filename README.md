# 用 Sinopia 搭建私有库


## 安装
npm install -g sinopia
sinopia <!-- 完成，访问：http://localhost:4873/ -->
npm set registry http://localhost:4873/ <!-- 修改 npm registry -->
<!-- npm set registry https://registry.npmjs.org/ -->


## 注册一个新的用户
npm adduser --registry http://localhost:4873/


## 发布
<!-- 本地私有库地址：/Users/jiezhiyong/.local/share/sinopia/storage -->
cd ~
mkdir -p tools/sinopia/local-example; cd tools/sinopia/local-example
npm init
npm publish


## 更新
cd ~/tools/sinopia/local-example
npm version 1.1.0
npm publish


## 删除
npm unpublish local-example --force


## 安装发布的本地私有库
npm i local-example

![Sinopia](http://upload-images.jianshu.io/upload_images/2445565-f0bd99c4ee127626.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240 "")
