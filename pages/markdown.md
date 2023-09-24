- [Markdownライティング入門](https://amzn.to/44NvqOx)より引用
	- > Markdownはプレーンテキストで文章を書くための記法
- Markdownの記法を試す
	- [[logseq]]特有の記法もある
- 見出し
	- # h1h1h1
	- ## h2h2h2
	- ### h3h3h3
	- #### h4h4h4
- inline系の記法
	- `**strong**` : **strong**
	- `*em*` : *em*
	- `~~strike~~` : ~~strike~~
	- `^^highlight^^` : ^^highlight^^
	- `$$E = mc^2$$` : $$E = mc^2$$
	- `` `code` ``  : `code`
	- `[link](url)` : [link](https://github.com/hachian/digital_garden)
	- `#tags`  : #tags
- block系の記法
	- ```python
	  import numpy as np
	  
	  def func():
	    pass
	  
	  a = 12
	  b = "aaa"
	  c = type(a)  # comment
	  ```
	- > 行の先頭に `>` を付けて引用
	  > 行の先頭に `>` を付けて引用
	- #+BEGIN_QUOTE
	  `#+BEGIN_QUOTE`で引用ブロックを始める
	  `#+END_QUOTE`で引用ブロックを終わる
	  `<`を押して、`quote`と検索するとできる
	  ブロック内での改行は`Shift+Enter`
	  #+END_QUOTE
	- query-table:: true
	  #+BEGIN_NOTE
	  `#+BEGIN_NOTE`でノートブロックを始める
	  `#+END_NOTE`でノートブロックを終わる
	  `<`を押して、`note`と検索するとできる
	  `IMPORTANT`、`PINNED`などいろいろある
	  #+END_NOTE
	- #+BEGIN_CENTER
	  `#+BEGIN_CENTER`で中央揃えブロックを始める
	  `#+END_CENTER`で中央揃えブロックを終わる
	  `<`を押して、`center`と検索するとできる
	  #+END_CENTER
- ショートカット(`/`;スラッシュ)系の記法
	- 日付系
		- [[2023/09/05]]などのリンクを生成
		- `/Today`, `/Yesterday`, `/Tomorrow`
	- TODO系
		- `TODO` : `/TODO`
		  :LOGBOOK:
		  CLOCK: [2023-09-06 Wed 22:46:08]--[2023-09-06 Wed 22:46:09] =>  00:00:01
		  :END:
		- DONE : `/DONE`
		  :LOGBOOK:
		  CLOCK: [2023-09-06 Wed 01:23:36]--[2023-09-06 Wed 01:23:36] =>  00:00:00
		  CLOCK: [2023-09-06 Wed 01:23:36]--[2023-09-06 Wed 01:23:37] =>  00:00:01
		  :END:
		- NOW : `/NOW`
		  :LOGBOOK:
		  CLOCK: [2023-09-06 Wed 01:23:48]
		  CLOCK: [2023-09-06 Wed 01:24:03]--[2023-09-06 Wed 01:24:13] =>  00:00:10
		  CLOCK: [2023-09-06 Wed 01:24:14]--[2023-09-06 Wed 01:24:15] =>  00:00:01
		  CLOCK: [2023-09-06 Wed 01:24:18]
		  :END:
		- LATER : `/LATER`
		  :LOGBOOK:
		  CLOCK: [2023-09-06 Wed 01:24:19]--[2023-09-06 Wed 01:24:19] =>  00:00:00
		  :END: