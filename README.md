# bleem-blog
## 介绍
基于docsify框架实现的超轻量级的博客方案，本项目解决以下痛点：
- 前端技术不咋滴（后端开发者）要非专业前端程序员也可以维护;
- 遇到问题在网上找思路时，每个平台都要求开通账号登录，验证...一套搞下来问题没解决，各个平台账号开了一大堆。
- 积累了很多年的markdown笔记记录着自己遇到的坑，不想一个个录入到各个博客网站上给他们引流收费，所以打算自己搞个博客平台。
- 开源: 一款软件，我要长久使用，那么不能是封闭的。如果哪一天应用作者不更新了，我要能自己 fork 一份来自己维持基本的运行;
- 可拓展: 这款应用要具备足够的拓展性，我遇到一些自己特定的需求，或者使用软件有不顺手的地方，我要能自己写插件或者拓展来修改和实现。
上面的原则都是为了让我可以长久使用一款博客平台。如果你认同上面的观点，那么 bleem-blog 或许是你的菜。
## 技术选型
- nodejs
- docsify
    - 动态编译机制
    - 灵活的插件架构
    - Markdown 扩展功能
## 使用
> 
1. 安装node：
1. 安装docsify：
    ```
    npm i docsify-cli -g

    ```
1. clone本项目：
    ```
    git clone git@github.com:RipleyGit/bleem-blog.git
    ```
1. 软连接md笔记：
    1. mac：
        1. 删除原docs文件夹：rm -rf docs
        1. 创建软连接：ln -s 你的笔记路径 ./docs
    1. linux: 创建软连接：ln -s 你的笔记路径 ./docs
1. 测试启动：docsify serve .
    ```
    docsify serve .
    Serving /Users/xxx/Documents/github/bleem-blog now.
    Listening at http://localhost:53603
    ```
1. 打开链接查看：http://localhost:53603