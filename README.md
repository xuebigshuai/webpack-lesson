# 一、 命令行参数  
````
webpack3.X
webpack index.js bundle.js  -p -d --progress
index.js 打包文件的入口路径 bundle.js打包生成的文件名


webpack4.x 版本 
  1、4.x版本需要手动安装webpack-cli 和webpack配套（同全局，同局部）
  2、默认打包到同级目录下的dist文件下main.js
webpack index.js
````
* webpack 开发环境下编译
* webpack -p 生产环境下编译，会压缩生成后的文件
* webpack -w 开发换环境下持续监听文件变动来进行编译
* webpack -d 生成map映射文件，会在控制台的source页签中出现存放打包前原始文件的webpack://目录，可以打断点调试
````
webpack index.js bundle.js -d
````
* webpack --progress 显示构建百分比进度
* webpack --display-error-details 显示打包过程中出现的错误信息
* webpack --profile 输出性能数据，可以看到每一步的耗时   
*************  一般不用命令行来进行打包*********************  
# 二、创建webpack配置文件 webpack.config.js
![](.README_images\ab84cd0b.png)