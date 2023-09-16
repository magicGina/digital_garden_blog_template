---
title: 某某某的博客_首页
dg-publish: true
dg-home: true
cssclasses:
  - cards
  - cards-cover
  - embed-strict
  - cards-1-1
  - cards-cols-4
---
# **HOME**
  hi,这里是某某某的博客
## 博文列表
```dataview
table WITHOUT ID ("![|100](" + cover + ")") as 封面, file.link as 博文, dateformat(create-date,"yyyy-MM-dd") as 日期, substring(file.folder,9)+" "+join(filter(file.tags, (x) => startswith(x, "#by"))," ") as 类型和作者 from #blog  and "00_blogs" sort create-date desc
```

## 未来计划

![[待办视图]]
