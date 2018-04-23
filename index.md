# 來自 GitHub Learning Labs 的學習課程

# 這是第一份 Markdown 文件
在 Visual Studio 代碼中使用 Markdown 文件很簡單，直接且有趣。除了 VS Code 的基本編輯外，還有許多 Markdown 特定功能可以幫助您提高工作效率。

This is Head 1（加 ===）
===

This is Head 2（加 ---）
---

在 Visual Studio 代碼中使用 Markdown 文件很簡單，直接且有趣。除了VS Code的基本編輯外，還有許多 Markdown 特定功能可以幫助您提高工作效率。
## 第二層標題
### 第三層標題
#### 第四層標題

# 一般文字

一個段落是由一個以上相連接的行句組成，
而一個以上的空行則會切分出不同的段落
（空行的定義是顯示上看起來像是空行，便會被視為空行。
比方說，若某一行只包含空白和tab，則該行也會被視為空行），
一般的段落不需要用空白或斷行縮排。
**（以上編寫時分行，但顯示為同一段落）**

「一個以上相連接的行句組成」  
這句話其實暗示了 Markdown 允許段落內的強迫斷行，  
如果你真的想要插入 &lt;br> 標籤的話，在行尾加上**兩個以上的空白**，然後按 ` enter `。

## 特殊字元
	<：&lt;
	&：&amp;
	著作權符號：&copy;

# 強調
東京*超市價*電爆台灣！經常赴日旅遊的**大學生**Sharon時常在分享生活點滴，日前她針對台灣與日本的物價做比較，以東京超市所販賣的便當為例，~~半價出清~~的便當竟__只要新台幣約50元__，但日本的薪資約台灣的2到3倍，相較之下，其實台灣物價反而比較高。

# 區塊引言
> Markdown 使用 email 形式的區塊引言，如果你很熟悉如何在 email 信件中引言，
> 你就知道怎麼在 Markdown 文件中建立一個區塊引言，那會看起來像是你強迫斷行，
> 然後在每行的最前面加上 >。
>> 區塊引言可以有階層（例如：引言內的引言），只要根據層數加上不同數量的 >。

引言的區塊內也可以使用其他的 Markdown 語法，包括標題、清單、程式碼區塊等：

> ## This is a header.
> 
> 1.   This is the first list item.
> 2.   This is the second list item.
> 
> Here's some example code:
> 
>     return shell_exec("echo $input | $markdown_script");

# 清單
1. 有序清單

	縮排（2~5 個空白或 1 個 tab）
	> 清單內也可以放引言

		<清單中的程式碼（比所屬清單層再縮進 2 個 tab）>

2. 第二點
	* 無序清單
	* 第二點
	+ 也可以用加號（+）
	- 也可以用減號（-）

			<清單中的程式碼（比所屬清單層再縮進 2 個 tab）>

**為了純文字檔排版好看，也可以使用縮排。**

清單項目標記通常是放在最左邊，也可以縮排，最多三個空白，項目標記後面則一定要接著至少一個空白或tab。要讓清單看起來更漂亮，你可以把內容用固定的縮排整理好：

* Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
  Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
  viverra nec, fringilla in, laoreet vitae, risus
* Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
  Suspendisse id sem consectetuer libero luctus adipiscing.

# 程式碼區塊

### 只要簡單地縮排 4 個空白或是 1 個 tab

	private setMode():void{
		var w = window.screen.availWidth;
		...
	}

### 或 前後用三個反引號包起來。

```
if(w >= 600){
	this.mode = this.SIDEMODE.SIDE;
	this.showSidenav = true;
}else{
	this.mode = this.SIDEMODE.OVER;
	this.showSidenav = false;
}
```

## 行內程式碼
如果要標記一小段行內程式碼，可以用反引號把它包起來，例如 ` return this.value; `。

如果要在程式碼區段內插入反引號，可以用多個反引號來開啟和結束程式碼區段，如 `` ` `` 。

## 避免不必要的清單

項目清單很可能會不小心產生，就是在行首出現**數字－句點－空白**，但我們不想變成清單。

1986. What a great season.

避免：在句點前面加上**反斜線**。

1986\. What a great season.

# 分隔線
你可以在一行中用**三個或以上**的星號、減號、底線來建立一個分隔線，行內不能有其他東西。也可以在星號中間插入空白。

--------------------------------

# 連結
## 行內形式

[這是一個行內連結](https://www.google.com)

[這是一個帶有標題的行內連結](https://www.google.com "Google's Homepage")

[相對參考連結](../blob/master/LICENSE)

## 參考形式
[這是一個參考連結][Arbitrary case-insensitive reference text]

[參考標的物也可以使用數字][1]

直接使用文字對應也可以 [這段文字連到參考項目]

參考項目可以寫在文檔的最後，有點像書內的註解（註腳）。

[arbitrary case-insensitive reference text]: https://www.mozilla.org
[1]: http://slashdot.org
[這段文字連到參考項目]: http://www.reddit.com



# HTML
非純文字內容者，可直接加上 HTML 撰寫。如：
<table>
	<tr>
		<td>儲存格 1</td>
		<td>儲存格 2</td>
		<td>儲存格 3</td>
	</tr>
</table>

# 其他

## 自動連結
Markdown 支援比較簡短的自動連結形式來處理網址和電子郵件信箱，只要是用角括號包起來，Markdown 就會自動把它轉成連結。

<https://www.google.com.tw/>

# 表格
**冒號** 是用來對齊的（擺左齊左、擺右齊右，都擺就置中）。
| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

最外圍的豎線（|）不是絕對需要，表格內也可以不用空白排版。

姓名|編號|email
|---|---|---
Eric Liu|001|test@gmail.com
Sangra Hsiung|002|welcome@hinet.net


# 圖片
很明顯地，要在純文字應用中設計一個「自然」的語法來插入圖片是有一定難度的。
Markdown 使用一種和連結很相似的語法來標記圖片，同樣也允許兩種樣式：行內和參考。

行內圖片的語法看起來像是：

![CKAC](images/FB.png "Optional title")

## 缺點
到目前為止， Markdown 還沒有辦法指定圖片的寬高，如果需要可以使用普通的 &lt;img> 標籤。
（但實測不行？？）
<img src="images/FB.png" width="778" height="778">
