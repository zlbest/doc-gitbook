## gitbook启动应用

1. 全局安装gitbook
   ```
   npm i gitbook-cli -g
   ```
2. 安装gitbook插件
   ```
   gitbook install
   ```
3. 启动gitbook开发模式
   ```
   gitbook serve
   ```
4. 打包gitbook应用
   ```
   gitbook build
   ```

## 项目目录结构

```
.
├── readme.md             //readme
├── introduction.md       //主页介绍
├── SUMMARY.md            //左侧目录
├── book.json             //gitbook配置文件
└── styles                //主题样式自定义
│   └── website.css       //web样式
├── assets                //图片资源等文件
│   ├── ...
├── _book                 //编译目录
│   ├── ...
├── component             //组件模块
│   ├── README.md         //组件介绍
│   ├── chapter1.md       //组件子目录1
│   └── chapter2.md       //组件子目录2
│   └── ...
├── framework
│   ├── README.md
│   ├── chapter1.md
│   └── chapter2.md
├── quick_start
│   ├── README.md
│   ├── chapter1.md
│   └── chapter2.md
├── ...
```
