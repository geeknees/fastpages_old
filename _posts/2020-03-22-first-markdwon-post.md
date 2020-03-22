---
toc: true
layout: post
description: fastpagesでmarkdownをの記事を投稿する
categories: [markdown]
title: Markdownを使った投稿の例（和訳）
---

# Markdown を使った投稿の例（和訳）

## 基本設定

Jekyll は下記のフォーマットで投稿する必要があります:

`YEAR-MONTH-DAY-filename.md`

`YEAR`は 4 桁の数字、`MONTH` と `DAY` は２桁の数字、 `filename` はどのようなフォーマットでも構いません。どのような内容かわかるものを記載してください。 末尾に `.md` の拡張子を追加してください。

ファルの最初の行は１つのハッシュ（シャープ）で始める必要があります。その後スペースを一ついれて、タイトルを記載してください。これはレベル１のヘッダーテキストを記載する方法です。ハッシュの数を増やすことで、上記の `## 基本の設定` のようにレベル２，３と変えることができます。

## 基本フォーマット

_イタリック_, **太字**, `コーテキスト`, [リンク](https://www.markdownguide.org/cheat-sheet/)を書くことができます。脚注は [^1] のように書きます。水平線は下記のように書きます。:

---

## リスト

これはリストです:

- item 1
- item 2

番号付きリストです:

1. item 1
1. item 2

## ボックス

> これは引用です

{% include alert.html text="アラートボックスに記入" %}

や

{% include info.html text="インフォボックスに記入" %}

もできます。

## 画像

![]({{ site.baseurl }}/images/logo.png "fast.ai's logo")

## コード

通常通りにコードを書くこともできます。

一般的なフォーマットされていないテキスト:

    # Do a thing
    do_thing()

Python のコードとその出力:

```python
# Prints '2'
print(1+1)
```

    2

shell コマンドとその出力:

```shell
echo "hello world"
./some_script.sh --option "value"
wget https://example.com/cat_photo1.png
```

YAML 形式で書かれたテキスト:

```yaml
key: value
- another_key: "another value"
```

## テーブル

| Column 1 | Column 2      |
| -------- | ------------- |
| A thing  | Another thing |

## Tweetcards

{% twitter https://twitter.com/jakevdp/status/1204765621767901185?s=20 %}

## 脚注

[^1]: これが脚注です。
