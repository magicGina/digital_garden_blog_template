---
title: test_dataview
dg-publish: false
---

```dataview
table WITHOUT ID file.link as 博文, dateformat(date,"yyyy-MM-dd") as 日期, substring(file.folder,9) as 类型,filter(file.tags, (x) => startswith(x, "#by")) as "作者" from #blog and"00_blogs" sort date desc
```