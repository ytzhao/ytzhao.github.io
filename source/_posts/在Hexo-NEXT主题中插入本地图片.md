---
title: 在Hexo NEXT主题中插入本地图片
date: 2020-11-08 16:02:57
tags:
---

# 前期准备

注意一定要安装下面这个版本的 ```hexo-asset-image```，否则图像还是会显示不正确。

```shell
npm install https://github.com/CodeFalling/hexo-asset-image --save
```

<!-- more -->

设置```your_blog_dir/_config.yml``` 中```post_asset_folder: true```

```shell
_posts/
|__ test.md
|__ test/
    |__ test.png
```

# 在.md文档中插入图像

```markdown
{% asset_img test.png This is an test image %}
<!-- 或者 --> 
![This is an test image](test.png)
```

