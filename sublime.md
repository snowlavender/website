#Sublime 指令教學

## 前言
sublime 是幾年在工程師世界裡最 popular 的編輯器，介面乾淨之外，可以自由幫它加上許許多多的外掛程式，讓它變得越來越好用。

## 操作
選取：[shift] + [方向鍵]
到行頭：[cmd] + [左]
到行尾：[cmd] + [尾]
到頁頭：[cmd] + [上]
到頁尾：[cmd] + [下]
用單字移動：[alt] + [方向鍵]
單字選取：對單字滑鼠點兩下
相同字重複選取：先選取某單字後，然後按 [cmd] + D，按幾次就選幾個。
把原始碼註解：[cmd] + /


## 套件
### Emmet
說明：它可以讓我們只要輸入標籤名+tab，就會自動產生雙標籤，例如：

```html
html + [tab] = <html></html>

body + [tab] = <body></body>

html>body + [tab] =
<html>
  <body>
  </body>
</html>

html>head+body + [tab] =
<html>
  <head>
  </head>
  <body>
  </body>
</html>

! + [tab] = 一個完整的空白網頁檔
```

#### 出現階層標籤
基本階層: ul>li + [tab] 會出現
```html
<ul>
  <li></li>
</ul>
```

階層內容: ul>li`{內容}` + [tab] 會出現
```html
<ul>
  <li>內容</li>
</ul>
```

重複階層: ul>li{內容}`*3` + [tab] 會出現
```html
<ul>
  <li>內容</li>
  <li>內容</li>
  <li>內容</li>
</ul>
```

重複階層序列: ul>li{內容`$`}*3 + [tab] 會出現
```html
<ul>
  <li>內容1</li>
  <li>內容2</li>
  <li>內容3</li>
</ul>
```

多階層: table>tr>td
```html
<table>
	<tr>
		<td></td>
	</tr>
</table>
```

範圍括孤: table>(tr>td*2)*3
```html
<table>
	<tr>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td></td>
		<td></td>
	</tr>
	<tr>
		<td></td>
		<td></td>
	</tr>
</table>
```

#### 出現隨機文章
lorem +[tab]

---
### AutoFileName
說明：在指定資源檔時，會自動幫我們列出目前檔案位置的檔案：
![autoFileName](http://files.rjwebdesign.cz/i/20140910-115755---595x346---t---pn.png "autoFileName")

---
### Color HighLighter
說明：自動幫我們秀出色碼代碼的顏色：
![Color HighLighter](https://camo.githubusercontent.com/e13f5346a650e7e3fc2269fd4de3904d78c8fd1e/687474703a2f2f692e696d6775722e636f6d2f55506d456b30392e706e67 "Color HighLighter")
