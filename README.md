# Markdown: 语法
markwodn 语法手册

- 概况

	- 宗旨
	- 内嵌HTML
	- 转义字符

- 块标记

	- 段落 & 换行
	- 头标题
	- 
	- 列表
	- 代码块
	- 分割线


# 概况

## 宗旨

Markdown是一种可行的易读易写的文本标记语法。当然易读性是最重要。一个标记格式的文档应该像纯文本一样是可发布的，而不象它被标记或格式化指令标记。虽然MalkScript的语法受到了一些现有文本到HTML过滤器的影响——包括SETXT、ATX、纺织、RealStudioDtext、GrutATEXT和ETtext——MalkDon语法的唯一最大灵感来源是纯文本电子邮件的格式。为此，标记的语法完全由标点符号组成，标点符号已经被仔细地选择，以便看起来像他们的意思。例如，围绕一个词的星号实际上看起来像*强调*。降价列表看起来很好，列表。甚至连块引文看起来都像是引用的文本段落，假设你曾经使用过电子邮件。

## 内嵌HTML

Markdown's syntax is intended for one purpose: to be used as a format for writing for the web.

Markdown is not a replacement for HTML, or even close to it. Its syntax is very small, corresponding only to a very small subset of HTML tags. The idea is not to create a syntax that makes it easier to insert HTML tags. In my opinion, HTML tags are already easy to insert. The idea for Markdown is to make it easy to read, write, and edit prose. HTML is a publishing format; Markdown is a writing format. Thus, Markdown's formatting syntax only addresses issues that can be conveyed in plain text.

For any markup that is not covered by Markdown's syntax, you simply use HTML itself. There's no need to preface it or delimit it to indicate that you're switching from Markdown to HTML; you just use the tags.

The only restrictions are that block-level HTML elements -- e.g. <div>, <table>, <pre>, <p>, etc. -- must be separated from surrounding content by blank lines, and the start and end tags of the block should not be indented with tabs or spaces. Markdown is smart enough not to add extra (unwanted) <p> tags around HTML block-level tags.

For example, to add an HTML table to a Markdown article:

This is a regular paragraph.


<table>
    <tr>
        <td>Foo</td>
    </tr>
</table>

This is another regular paragraph.



# 块元素

## 段落和换行

`<br />`


## 头标题


`
这是H1
====== 

这是H2
------

`
# 这是H1 

## 这是H2

`

`
# 这是H1 #

## 这是H2 ##

`



## 列表

Markdown支持有序（编号）和无序列表

`
* 红
* 黄
* 蓝
`
或者: <br />
`
+ 红
+ 黄
+ 蓝
`
或者: <br />
`
- 红
- 黄
- 蓝
`
有序编号
`
1. 红
2. 黄
3. 蓝
`
或者：<br />

`
1. 红
1. 黄
1. 蓝
`


## 分割线

`
* * *

***

*****

- - -

------------------------
`

# 行元素

## 链接

`
这是一个[链接](https://albenyuan.com, 'Alben Yuan')

这个[链接](https://albenyuan.com)没有标题

`

## 加重

`
*强调*

-强调-

**强调**

__强调__
`

## 代码

```这是一个代码：`println()` ```

## 图片

`![Alt](/path/to/img.jpg, 'Title')`







