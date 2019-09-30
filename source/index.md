title: 项目说明
---

## 基础环境

`node >= 6.0.0
npm >= 3.0.0`

## 初始化

 - Clone or download this repository
 - Enter your local directory, and install dependencies:

``` bash
npm install
```

## 开发运行

``` bash
# serve with hot reload at localhost:8010
npm run dev
```

## 编译构建

``` bash
# build for production with minification
npm run build
```

## 目录结构

```
├── config                         -- 构建脚本目录
│   ├── env                        ---- 项目配置目录
│   │   ├── dev.env.js             ------ 开发环境变量
│   │   ├── index.js               ------ 项目配置文件
│   │   ├── prod.env.js            ------ 生产环境变量
│   │   └── test.env.js            ------ 测试环境变量
│   ├── build.js                   ---- 构建脚本
│   ├── check-versions.js          ---- 版本检测
│   ├── utils.js                   ---- 构建相关工具
│   ├── webpack.base.conf.js       ---- wabpack基础配置
│   ├── webpack.dev.conf.js        ---- wabpack开发环境配置
│   └── webpack.prod.conf.js       ---- wabpack生产环境配置
├── src                            -- 项目源码目录    
│   ├── main.js                    ---- 入口脚本
│   ├── App.vue                    ---- 根组件
│   ├── assets                     ---- 资源目录，这里的资源会被wabpack构建
│   │   ├── images                 ------ 图片资源
│   │   ├── lang                   ------ 国际化处理资源
│   │   ├── mock                   ------ 模拟数据仓库
│   │   └── repos                  ------ 数据仓库
│   ├── scripts                    ---- 脚本资源
│   │   ├── routes                 ------ 前端路由
│   │   └── store                  ------ 应用数据（state）
│   └── view                       ---- 页面目录
│       ├── components             ------ 公共组件
│       └── modules                ------ 业务模块相关
├── static                         -- 纯静态资源，不会被wabpack构建
├── favicon.ico                    -- 网站图标
└── package.json                   -- npm包配置文件，里面定义了项目的npm脚本，依赖包等信息
```

