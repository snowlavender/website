#CSS 教學

## 前言
css 是網頁的樣式修飾語言，語法與 html 不同。主要是在幫網頁標籤加上不同的樣式，像是顏色、大小、對齊…等，看得到的都是它可以處理的。
>網路上甘有一個人很無聊用 css 刻了一個哆啦a夢出來：http://purecss3.net/doraemon/doraemon_css3.html

## inline style
說明：直接在 html 標籤上使用，直接影響該標籤

```html
<span style="color: red"> 我是紅字 </span>
```

你也可以一次用多指令
```html
<span style="color: red; background-color: yellow"> 我是黃底紅字 </span>
```

如此一來，我們就可以為 html 設定各式各樣的樣子，如果我們有兩個相同樣式的標籤，它可能長這樣：

```html
<span style="color: red; background-color: yellow; "> 我是黃底紅字 1</span>
<span style="color: red; background-color: yellow; "> 我是黃底紅字 2</span>
```

如果今天我們希望把紅字都改成「藍字」那你需要改2次，這不打緊。但如果今天有100個標籤都希望改成藍字，那我們就有得忙了。

所以通常，我們會把它另外寫成一個樣式表，以便我們方便修改。

## class style
說明：在 haad 裡使用 style 標籤，然後定義樣式：

```html
<head>
  <style>
    .myspan{
		color: red;
		background-color: yellow;
    }
  </style>
</head>
```
如上所見，我們定義了一個叫 `.myspan` 的class，所以我們可以把原先的 2 個 `span` 直接套用這個 `.myspan`

```html
<span class="myspan"> 我是黃底紅字 1</span>
<span class="myspan"> 我是黃底紅字 2</span>
```


所以完整的檔案看起來會像這樣

```html
<html>
  <head>
    <style>
      .myspan{
		  color: red;
		  background-color: yellow;
      }
    </style>
  </head>
  <body>
  	  <span class="myspan"> 我是黃底紅字 1</span>
	  <span class="myspan"> 我是黃底紅字 2</span>
  </body>
</html>
```

如此一來，以後如果要改字的顏色，我們只需到 `.myspan` 把它的 color  改成我們要的顏色，那所有套用 `.myspan` 的標籤就會直接套用了！不必再一一修改！

