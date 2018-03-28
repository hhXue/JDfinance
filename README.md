### 组件式开发

##### 文件app目录
```
├── css  //css抽象
│   ├── element.scss
│   ├── layout.scss
│   └── reset.scss
│
├── js	
│    ├── core  //核心组件
│        ├── btn.vue     //按钮
│        ├── panel.vue   //面板
│        └── slider.vue  //轮播图
│    ├── home    //首页组件
│    ├── ious    //白条组件
│    ├── money   //理财组件
│    ├── public  //公共组件 
│    ├── raise   //众筹组件
│    ├── router  
│        └── index.js //路由配置
│    ├── App.vue
│    ├── main.js      //入口文件
│    ├── package.json //包依赖文件
│    └── viewport.js  //px2rem
│    
└── views	//视图
    └── index.html
```

#### 项目注意点
- 自适应方案 —— github中hotcss终极版方案 需要看看
    参考：http://www.dailibu.com/html-css/20160520187/DongTaiJiSuanhtmlDefont-size
    自动化适配，不需要考虑多设备，只根据当前设备设置，其他设备自动适配！！！！！

- slider开源的组件 vue-awesome-swiper

- 布局要先整体，再局部

- icon 图标不用图片，用图标 字体文件
