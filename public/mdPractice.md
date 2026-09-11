---
title: mdファイルの記述練習
tags:
  - Markdown
  - 練習
private: false
updated_at: '2026-09-11T13:07:46+09:00'
id: 0eda749eba98626a4525
organization_url_name: null
slide: false
ignorePublish: false
posting_campaign_uuid: null
agreed_posting_campaign_term: false
---
# 見出しの記入例
~~~
#     見出しレベル1
##    見出しレベル2
###   見出しレベル3
####  見出しレベル4
##### 見出しレベル5

見出しレベル1
========

見出しレベル2
--------
~~~

# テキストの装飾
## 強調表示
強調したいテキストを`**`で囲む  
強調したい**テキスト**を`**`で囲む
~~~
強調したい**テキスト**を`**`で囲む
~~~

## 斜体表示
斜体で表示したいテキストを`*`で囲む  
斜体で表示したい*テキスト*を`*`で囲む
~~~
斜体で表示したい*テキスト*を`*`で囲む
~~~

## 打消し線
打消し線を引きたいテキストを`~~`で囲む  
打消し線を引きたい~~テキスト~~を`~~`で囲む
~~~
打消し線を引きたい~~テキスト~~を`~~`で囲む
~~~

## 下線
下線を引きたいテキストは`<ins></ins>`で囲む  
下線を引きたい<ins>テキスト</ins>は`<ins></ins>`で囲む
~~~
下線を引きたい<ins>テキスト</ins>は`<ins></ins>`で囲む
~~~

## 文字の色とサイズ
テキストに対してMathJax`$\color{red}{\large{テキスト}}$`で指定する  
$\color{red}{\large{テキスト}}$に対してMathJax`$\color{red}{\large{テキスト}}$`で指定する[^1]
~~~
$\color{red}{\large{テキスト}}$に対してMathJax`$\color{red}{\large{テキスト}}$`で指定する
~~~
### 色だけの変更
テキストに対してタグ`<font color=red></font>`を使用する  
<font color=red>テキスト</font>に対してタグ`<font color=red></font>`を使用する
~~~
<font color=red>テキスト</font>に対してタグ`<font color=red></font>`を使用する
~~~

[^1]:Qiita上では見出しタグまたはMathJax以外のサイズの変更が不可能

# テーブルの記述
~~~
|Left|Center|Right|
|:---|:----:|----:|
|This|This|This|
|column|column|column|
|is|is|is|
|left|center|right|
|aligned|aligned|aligned|
~~~
|Left|Center|Right|
|:---|:----:|----:|
|This|This|This|
|column|column|column|
|is|is|is|
|left|center|right|
|aligned|aligned|aligned|

## セルの結合
HTMLを使用することによって結合可能  
3x4 table
~~~html:sample
<table>
  <tr>
    <th>ヘッダー１</th>
    <th colspan=2>ヘッダー２</th>
  </tr>
  <tr>
    <td>a</td>
    <td>1</td>
    <td>2</td>
  </tr>
  <tr>
    <td rowspan=2>b</td>
    <td>1</td>
    <td>2</td>
  </tr>
  <tr>
    <td>1</td>
    <td>2</td>
  </tr>
</table>
~~~
<table>
  <tr>
    <th>ヘッダー１</th>
    <th colspan=2>ヘッダー２</th>
  </tr>
  <tr>
    <td>a</td>
    <td>1</td>
    <td>2</td>
  </tr>
  <tr>
    <td rowspan=2>b</td>
    <td>1</td>
    <td>2</td>
  </tr>
  <tr>
    <td>1</td>
    <td>2</td>
  </tr>
</table>
