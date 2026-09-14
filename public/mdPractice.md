---
title: mdファイルの記述練習
tags:
  - Markdown
  - 練習
private: false
updated_at: ''
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

## 上付き・下付き文字
### 下付き
<sub>テキスト</sub>を`<sub></sub>`で囲むと下付きにできる
~~~
<sub>テキスト</sub>を`<sub></sub>`で囲むと下付きにできる
~~~

### 上付き
<sup>テキスト</sup>を`<sup></sup>`で囲むと上付きにできる
~~~
<sup>テキスト</sup>を`<sup></sup>`で囲むと上付きにできる
~~~

[^1]:Qiita上では見出しタグまたはMathJax以外のサイズの変更が不可能

# テーブルの記述
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
~~~

## セルの結合
HTMLを使用することによって結合可能  
3x4 table

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

# リスト
## 箇条書きリスト
- 1
  - A
    - a
- 2
  - B
    - b
- 3
  - C
    - c
~~~
- 1
  - A
    - a
- 2
  - B
    - b
- 3
  - C
    - c
~~~

## 番号付きリスト
番号は自動で振られる、
1. 一
2. 二
    1. a
  3. 三
0. 四

~~~
1. 一
2. 二
    1. a
  3. 三
0. 四
~~~

# コード
## インラインコード
`インライン`を使用
~~~
`インライン`を使用
~~~

## コードブロック
### インデントによるコードブロック

    code by indent

### フェンスコードブロック
`~~~`で上下を挟むことでブロック化する
~~~
code by fence
~~~

#### シンタックスハイライト
上部の`~~~`の横に使用言語を記入することでハイライトできる
~~~c
// C言語のシンタックスハイライト
int main(void){
  int a = 2;
  char spell[4] = {Hello, World};
  for(i=0; i < a; i++){
    printf("%c", spell);
  }
  printf("!");
}
~~~

# 折りたたみ
<details>
  <summary>
    summaryで最初から表示しておきたい文章を表示できる
  </summary>
  detialsで囲った文章は折りたたまれる
</details>

~~~
<details>
  <summary>
    summaryで最初から表示しておきたい文章を表示できる
  </summary>
  detialsで囲った文章は折りたたまれる
</details>
~~~

# 引用
`>`で引用デザインにできる
>引用
>>ネストも可能
~~~
>引用
>>ネストも可能
~~~
