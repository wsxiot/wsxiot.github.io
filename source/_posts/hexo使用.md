---
title: hexo使用
date: 2017-11-13 14:18:30
tags:
- blog
- hexo
categories: tool
---

- 安装nodejs，git

- ```
  $ npm install -g hexo-cli #安装hexo
  ```

- ```
  $ hexo init #初始化hexo
  ```

- ```
  #修改主目录下_config.yml成这样
  deploy:
       type: git
       repo: https://github.com/yourname/yourname.github.io.git
       branch: master
  ```

- ```
  $ npm install hexo-deployer-git --save
  ```

- ```
  post_asset_folder: true #修改主目录下_config.yml成这样
  ```

- ```
  #这一条和上一条是为了能引用自己的图片
  npm install https://github.com/CodeFalling/hexo-asset-image --save
  #确保在/source/_posts下创建和md文件同名的目录，在里面放该md需要的图片，然后在md中插入
  ![](目录名/文件名.png)
  ```

-  ```
  $ hexo new "My New Post"
  ```

- ```
  #使用多个tag
  title: hexo使用
  date: 2017-11-13 14:18:30
  tags:
  - blog
  - hexo
  categories: tool
  ```

- ```
  $ hexo clean #清空上一次生成的文件
  ```

- ```
  $ hexo server #本地测试
  ```

- ```
  $ hexo generate #生成网站文件
  ```

- ```
  $ hexo deploy #部署
  ```