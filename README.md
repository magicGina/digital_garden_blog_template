# 基于Obsidian的Digital Garden插件的博客模板

## 效果
首页展示内容如下：

- 博文以卡片形式展示
- 展示了当前未完成的待办
- 简易的图床
    
效果见下图：

![image](https://github.com/magicGina/digital_garden_blog_template/assets/88796282/ca2b672e-6328-4e10-86e4-5630d05fe4eb)
![image](https://github.com/magicGina/digital_garden_blog_template/assets/88796282/2e8dc8ec-b9ea-4926-a267-8cf4722efc24)
<img width="518" alt="1695565389005" src="https://github.com/magicGina/digital_garden_blog_template/assets/88796282/80ff9c03-b46b-4316-9162-700e05529f87">


## 操作指南
这个博客也依赖于Minimal主题，另外，其他的插件如Templater等也在后期写博客过程中能用到，可以在以下链接取得： [下载配置好的插件包](https://miya.teracloud.jp/share/11d129ab6aa52054) 。直接解压到.obsidian文件夹下然后把插件全部开启就好。

有一些自定义的njk和css，保存在这个项目里了[user css and njk](https://github.com/magicGina/user_digitalgarden_setting)。简易的图床功能是需要某个njk的，请自己找找吧XD。

### 部署项目

**本项目只包含笔记内容，请勿依托本仓库进行站点构建，而应该只把它放到Obsidian中作为笔记模板使用**

还是应该按照 [digitalgarden官方文档](https://dg-docs.ole.dev/) 中的教程，以 [digitalgarden官方模板项目](https://github.com/oleeskild/digitalgarden) 为基础进行构建。本项目只是一个笔记模板，只应该把它放到本地Obsidian仓库中作为笔记使用。

如果使用了本项目作为本地笔记，并且使用了上面链接中的插件包，在Obsidian本地配置方面，就只剩下Digital Garden插件的git仓库选项需要配置了。输入你git仓库的相关配置就好。其中项目名称就是你根据 [digitalgarden官方模板项目](https://github.com/oleeskild/digitalgarden) 创建的github仓库（而非本仓库）。


就是只需要填写下图这三个框：
![image](https://github.com/magicGina/digital_garden_blog_template/assets/88796282/a933d03c-a7e6-4f46-a8d5-412a6c724c85)
### 添加文章
请见[添加文章教程](https://perch.parasoltree.top/00_blogs/%E5%BB%BA%E7%AB%99/%E4%BD%BF%E7%94%A8%E6%8C%87%E5%8D%97/%E6%B7%BB%E5%8A%A0%E6%96%87%E7%AB%A0/)

## 其他的一些话
这个模板也包含时间轴视图，但是目前Digital Garden还没有支持Timelines插件，这就造成了时间轴在笔记中显示但是在网页上不显示，是正常的！等待开发者大大们更新~

真的感谢Digital Garden的开发者们，让我能够非常方便地创建自己的小站，让不论接没接触过代码的朋友们都能享受其中！
