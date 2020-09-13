---
home: true
heroImage: /favicon.ico
actionText: 快速上手 →
actionLink: /guide/
features:
- title: 简洁至上0
  details: 以 Markdown 为中心的项目结构，以最少的配置帮助你专注于写作。
- title: Vue驱动
  details: 享受 Vue + webpack 的开发体验，在 Markdown 中使用 Vue 组件，同时可以使用 Vue 来开发自定义主题。
- title: 高性能
  details: VuePress 为每个页面预渲染生成静态的 HTML，同时在页面被加载的时候，将作为 SPA 运行。
- title: 高性能2
  details: VuePress 为每个页面预渲染生成静态的 HTML，同时在页面被加载的时候，将作为 SPA 运行。
- title: 高性能3
  details: VuePress 为每个页面预渲染生成静态的 HTML，同时在页面被加载的时候，将作为 SPA 运行。  
footer: MIT Licensed | Copyright © 2018-present xxxxxx
---

``` js
export default{
    data(){
        return {
            msg:'Highlighted!'
        }
    }
}
```
vuepress默认支持[PWA](https://segmentfault.com/a/1190000012353473),配置方法如下：
config.js 文件中增加
``` js
head: [ // 注入到当前页面的 HTML <head> 中的标签
  ['link', { rel: 'manifest', href: '/photo.jpg' }],
  ['link', { rel: 'apple-touch-icon', href: '/photo.jpg' }],
],
serviceWorker: true // 是否开启 PWA
```

public 文件夹下新建 manifest.json 文件，添加
``` json
{
  "name": "张三",
  "short_name": "张三",
  "start_url": "index.html",
  "display": "standalone",
  "background_color": "#2196f3",
  "description": "张三的个人主页",
  "theme_color": "blue",
  "icons": [
    {
      "src": "./photo.jpg",
      "sizes": "144x144",
      "type": "image/png"
    }
  ],
  "related_applications": [
    {
      "platform": "web"
    },
    {
      "platform": "play",
      "url": "https://play.google.com/store/apps/details?id=cheeaun.hackerweb"
    }
  ]
}
```
最后在 iPhone 的 safrai 浏览器中打开本网站，点击 +添加到主屏幕 就能在桌面看到一个像原生 App 一样的图标（感觉自己写了一个 App 有木有 smile）


::: tip 提示
this is a tip
:::

::: warning 注意
this is a tip
:::

::: danger 警告
this is a tip
:::

:tada: :100: :bamboo: :gift_heart: :fire: :moneybag:    
