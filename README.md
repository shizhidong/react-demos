##webpack
1.安装webpack
    npm install webpack --save-dev(不是全局安装)
    npm install webpack -g(全局安装)
2.新建webpack.config.js
    touch webpack.config.js
3.配置webpack.config.js
    打开webpack.config.js
    module.exports = {
      entry: __dirname + '/src/index.js',//编译路径
      output: {//输出路径
        path: __dirname + '/build',
        filename: 'bundle.js'
      }
    }
4.配置package.json
//新增这个配置文件用于运行编译文件配置好，就能运行 npm run build
//不配置需要全局安装webpack，运行 webpack就能编译
//-w是持续监听，ctrl+c中断监听
"scripts": {
  "build":"webpack"
},
4.启动服务
