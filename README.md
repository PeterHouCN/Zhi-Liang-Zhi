# 《致良知》
《致良知》学习笔记
使用Github制作。
Markdown语法参考https://daringfireball.net/projects/markdown/syntax

## 如何添加脚注？
### 法1
You can make the footnote links clickable here as well. First define the footnote at the bottom like this
```
<a name="myfootnote1">1</a>: Footnote content goes here
```
Then reference it at some other place in the document like this
```
<sup>[1](#myfootnote1)</sup>
```
### 法2

Expanding on the previous answers even further, you can add an id attribute to your footnote's link:
```
 Bla bla <sup id="a1">[1](#f1)</sup>
 ```
Then from within the footnote, link back to it.
```
<b id="f1">1</b> Footnote content here. [↩](#a1)
```
This will add a little ↩ at the end of your footnote's content, which takes your readers back to the line containing the footnote's link.
