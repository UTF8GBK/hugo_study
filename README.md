
# README

### 仿照https://brokers.fx110.com/  页面，实现展示经销商列表，点击经销商能够匹对应的json文件夹的数据进行渲染

#### 前期准备工作
- 打开https://brokers.fx110.com/，ctrl+s 保存html源码和静态文件
- 使用` hugo new site xxxx(站点名称)` 生成一个静态页面
- 创建一个空的主题 
- 在config配置文件中添加使用主题的命令 `theme : clarityii(主题名字)`
- 把刚才扒别人的html源码放在主题下面的partials文件夹下面，html名字任意取，尽量不好中文
- 把刚才扒别人的静态文件放到主题下面的static文件夹，css文件要创建一个css文件夹装起来，以此类推
- 修改html源码静态文件路径  hugo静态路径表达式  `/css/xxxx.css` `/js/xxxx.js`


#### 文件结构
```
├─.idea
│  └─inspectionProfiles
├─archetypes
├─assets
├─content   # 暂时不需要
│  └─trade_
├─data      # 存放json数据
├─layouts   # 暂时不需要
├─public    # 暂时不需要
├─resources 
│  └─_gen
│      ├─assets
│      └─images
├─static
│  ├─css
│  ├─images
│  └─js
└─themes    #主题文件
    └─clarityii
        ├─archetypes
        ├─layouts
        │  ├─partials   # 存放扒下来的源码
        │  └─_default
        └─static   # 扒别人的静态文件存放地
            ├─css
            ├─images
            └─js

```

#### 使用语法
xxxxx