---
title: cover-pictures
dg-publish: true
create-date: 2023-09-18T21:13:30.000+08:00
cssclasses:
  - table-wide
  - row-alt
---
# 这里是所有使用内部链接的标题图片，你可以复制链接来查看原图和使用

```dataviewjs
// 创建表格
let names = dv.pages('#blog').sort(b => b["create-date"],"desc").where(p=>(""+p.cover).endsWith("]]")).map(p=>[p.file.name,
"!\[\["+(""+p.cover).replace(/[!\[\]]|\|.*/g, "")+"|100\]\]"
,
	"<input type=\"text\" value=\""
	+ "https://perch.parasoltree.top/img/user/"+(""+p.cover).replace(/[!\[\]]|\|.*/g, "")
	+"\">"
	+"<button class=\"btn-copy-1\" type=\"button\">复制</button>"
]);
let markdown = dv.markdownTable(["文件名","图片","图片链接"],names);
dv.paragraph(markdown);

// 实现复制按钮的功能
function init_copy_btns(){
	let copy_btns = document.getElementsByClassName('btn-copy-1');
	for(let copy_btn of copy_btns){
		copy_btn.onclick = function(){
			let copy_input = copy_btn.previousSibling;
			try {
				navigator.clipboard.writeText(copy_input.value);
			} catch (err) {
				copy_input.select();
				document.execCommand('copy');
			}
		}
	}
}
setTimeout(init_copy_btns, 1000);
```
