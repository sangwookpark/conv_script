---
layout: base
title: Github pages 테스트
toc: true
---

------
# h1 Heading 8-)
## h2 Heading
### h3 Heading
#### h4 Heading
##### h5 Heading
###### h6 Heading


## Horizontal Rules

___

---

***


## Typographic replacements

Enable typographer option to see result.

(c) (C) (r) (R) (tm) (TM) (p) (P) +-

test.. test... test..... test?..... test!....

!!!!!! ???? ,,  -- ---

"Smartypants, double quotes" and 'single quotes'


## Emphasis

**This is bold text**

__This is bold text__

*This is italic text*

_This is italic text_

~Strikethrough~~


## Blockquotes


> Blockquotes can also be nested...
>> ...by using additional greater-than signs right next to each other...
> > > ...or with spaces between arrows.


## Lists

Unordered

+ Create a list by starting a line with `+`, `-`, or `*`
+ Sub-lists are made by indenting 2 spaces:
  - Marker character change forces new list start:
    * Ac tristique libero volutpat at
    + Facilisis in pretium nisl aliquet
    - Nulla volutpat aliquam velit
+ Very easy!

Ordered

1. Lorem ipsum dolor sit amet
2. Consectetur adipiscing elit
3. Integer molestie lorem at massa


1. You can use sequential numbers...
1. ...or keep all the numbers as `1.`

Start numbering with offset:

57. foo
1. bar


## Code

Inline `code`

Indented code

    // Some comments
    line 1 of code
    line 2 of code
    line 3 of code


Block code "fences"

```
Sample text here...
```

Syntax highlighting

``` js
var foo = function (bar) {
  return bar++;
};

console.log(foo(5));
```

``` js
<script type="text/javascript">
var foo = function (bar) {
  return bar++;
};
</script>
```


``` html
<script type="text/javascript">

 if (window.wcs) {
    // (2) 각 사이트별 식별자 설정
    wcs_add["wa"] = "AccountId";

    // (5) 결제완료 전환 이벤트 전송
    var _conv = {}; // 이벤트 정보 담을 object 생성

    _conv.type = 'purchase';  // object에 구매(purchase) 이벤트 세팅

    _conv.items = ... // 구매(purchase) 이벤트에 대한 세부 내용(Property) 세팅

    wcs.trans(_conv); // 전환 이벤트 정보를 담은 object를 서버에 전송
  }

</script>
```

## Tables

| Option | Description |
| ------ | ----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

Right aligned columns

| Option | Description |
| ------:| -----------:|
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

| **Property항목** | **세부항목** | **Data Type** | **의미** | **예시** | **Script예제** |
| ---- | ---- | ---- | ---- | ---- | ---- |
| id |  | string | 해당 전환 이벤트의 이용자 행동 ID. (광고주 사이트에서 생성>하는 정보) | 주문번호: 20231220 | _conv.id: '20231220' |
| items(#1) | item.id | string | 행동의 대상이 되는 재화/용역의 ID (예: 상품ID) | 상품번호: 7789 | \_conv.items=[<br/>  {  <br/>    id:'7786',  <br/>    name:'설화수 탄력크림',  <br/>    category:'화장품/스킨케어/크림',  <br/>    quantity:3,  <br/>    payAmount:90000,  <br/>    option: '용량:120',  <br/>  }<br/>] |
| ^ | item.name | string | 행동의 대상이 되는 재화/용역의 이름 | 상품명: 설화>수 탄력크림 | ^ |
| ^ | item.category | string | 재화/용역의 카테고리 | 카테고리: 화장품/스킨케>어/크림 | ^ |
| ^ | item.quantity | number | 재화/용역의 수량 | 구매(결제)수량: 3개 | ^ |
| ^ | item.payAmount | number | 재화/용역의 금액 (위 재화/용역 ID에 대한 총 결
제금액. 단가 아님) | 결제금액: 90,000원 | ^ |
| ^ | item.option | string | 재화/용역의 옵션 | 용량: 120ml | ^ |
| items(#2) | (위 #1 내용 반복) | ... |  |  |  |
| value |  | string | 복수개의 재화/용역의 전체 금액 (배송비 제외 권장) | 결제
금액: 50,000원 | _conv.value='50000' |

## Links

[link text](http://dev.nodeca.com)

[link with title](http://nodeca.github.io/pica/demo/ "title text!")

Autoconverted link https://github.com/nodeca/pica (enable linkify to see)


## Images

![Minion](https://octodex.github.com/images/minion.png)
![Stormtroopocat](https://octodex.github.com/images/stormtroopocat.jpg "The Stormtroopocat")

Like links, Images also have a footnote style syntax

![Alt text][id]

With a reference later in the document defining the URL location:

[id]: https://octodex.github.com/images/dojocat.jpg  "The Dojocat"


## Plugins

The killer feature of `markdown-it` is very effective support of
[syntax plugins](https://www.npmjs.org/browse/keyword/markdown-it-plugin).


### [Emojies](https://github.com/markdown-it/markdown-it-emoji)

> Classic markup: :wink: :cry: :laughing: :yum:
>
> Shortcuts (emoticons): :-) :-( 8-) ;)

see [how to change output](https://github.com/markdown-it/markdown-it-emoji#change-output) with twemoji.


### [Subscript](https://github.com/markdown-it/markdown-it-sub) / [Superscript](https://github.com/markdown-it/markdown-it-sup)

- 19^th^
- H~2~O


### [\<ins>](https://github.com/markdown-it/markdown-it-ins)

++Inserted text++


### [\<mark>](https://github.com/markdown-it/markdown-it-mark)

==Marked text==


### [Footnotes](https://github.com/markdown-it/markdown-it-footnote)

Footnote 1 link[^first].

Footnote 2 link[^second].

Inline footnote^[Text of inline footnote] definition.

Duplicated footnote reference[^second].

[^first]: Footnote **can have markup**

    and multiple paragraphs.

[^second]: Footnote text.


### [Definition lists](https://github.com/markdown-it/markdown-it-deflist)

Term 1

:   Definition 1
with lazy continuation.

Term 2 with *inline markup*

:   Definition 2

        { some code, part of Definition 2 }

    Third paragraph of definition 2.

_Compact style:_

Term 1
  ~ Definition 1

Term 2
  ~ Definition 2a
  ~ Definition 2b


### [Abbreviations](https://github.com/markdown-it/markdown-it-abbr)

This is HTML abbreviation example.

It converts "HTML", but keep intact partial entries like "xxxHTMLyyy" and so on.

*[HTML]: Hyper Text Markup Language

### [Custom containers](https://github.com/markdown-it/markdown-it-container)

::: warning
*here be dragons*
:::
