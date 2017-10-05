# vue-todos

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build
```

For detailed explanation on how things work, consult the [docs for vue-loader](http://vuejs.github.io/vue-loader).

# 首先在机器装安装npm 然后输入以下指令将vue-cli安装到机器的全局环境中
```
npm install vue-cli -g
```

>然后基于vue-cli创建一个project

```
vue init webpack-simple project-name
```

>此时控制台会提出一些关于新建项目的基本问题 可直接回车键跳过 然后进行以下操作

```
cd project-name
npm install
npm run dev
```

>npm install 指令是依据packge.json文件加载项目依赖库
>npm run dev 运行通过vue-cli脚手架创建的vue程序


>目录描述
>|--node_modules        #工程依赖的库 执行 npn install 自动生成
>|--src                 #开发目录
>|  |--assets           #组件
>|  |--App.vue
>|  |--main.js          #Vue实例启动入口
>|--index.html          #默认启动页面
>|--packge.json         #npm 包配置文件
>|--webpack.config.js   #webpack 配置文件
>|--README.md           #工程描述文件

>使用时间格式化库 moment

```
npm install moment -S
```

>  使用filters进行模版格式化 过滤器的实质上是一个只带单一输入参数的函数 过滤器有用的地方是可以管
>道方式进行传递调用 在vue组件中加入自定义过滤器 在filters属性内部 加入方法定义 就可以在模块上使用
>了














































































