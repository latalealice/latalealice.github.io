---
permalink: /markdown/
title: "Markdown"
author_profile: true
redirect_from: 
  - /md/
  - /markdown.html
---

## 关键文件/目录的位置

* 基本配置选项：_config.yml  
* 顶部导航栏配置：_data/navigation.yml  
* 单个页面：_pages/  
* 页面集合为.md或.html文件，位于：  
* _publications/  
* _portfolio/  
* _posts/  
* _teaching/  
* _talks/  
* 页脚_includes/footer.html  
* 静态文件（如PDF）：/files/  
* 头像（可在_config.yml中设置）：images/profile.png  

## 提示和技巧

* 将文件命名为“.md”以Markdown格式渲染，命名为“.html”以HTML格式渲染
* 前往代码库[commit list](https://github.com/academicpages/academicpages.github.io/commits/master)中的提交列表，查找Github使用Jekyll构建的最新版本
  * 绿色勾选：构建成功
  * 橙色圆圈：正在构建
  * 红色 X：错误
  * 无图标：未构建

## 资源配置
 * [Liquid syntax guide](https://shopify.github.io/liquid/tags/control-flow/)
 * [MathJax Documentation](https://docs.mathjax.org/en/latest/)

## 数学符号

模板中包含对MathJax3.0版的支持：

$$
\displaylines{
\nabla \cdot E= \frac{\rho}{\epsilon_0} \\\
\nabla \cdot B=0 \\\
\nabla \times E= -\partial_tB \\\
\nabla \times B  = \mu_0 \left(J + \varepsilon_0 \partial_t E \right)
}
$$

显示数学表达式时，支持默认分隔符 `$$...$$` 和 `\\[...\\]`，而内联数学表达式则应使用 `\\(...\\)`

**注意** 尽管有一些[解决方法](https://math.codidact.com/posts/278763/278772#answer-278772)，但还是要注意：由于Academic Pages使用Markdown，因此在转义字符和换行符方面会对MathJax和LaTeX造成一些干扰

## Markdown 指南

Academic Pages 使用 [kramdown](https://kramdown.gettalong.org/index.html) 进行 Markdown 渲染，这与 GitHub 等其他 Markdown 实现略有不同。除了本指南外，请参阅 [kramdown 语法页面](https://kramdown.gettalong.org/syntax.html) 获取完整文档

### 标题三

#### 标题四

##### 标题五

###### 标题六

## 区块引用

单行区块引用：

> 引用很酷

## 表格

### 表1

| Entry            | Item   |                                                              |
| --------         | ------ | ------------------------------------------------------------ |
| [John Doe](#)    | 2016   | Description of the item in the list                          |
| [Jane Doe](#)    | 2019   | Description of the item in the list                          |
| [Doe Doe](#)     | 2022   | Description of the item in the list                          |

### 表2

| Header1 | Header2 | Header3 |
|:--------|:-------:|--------:|
| cell1   | cell2   | cell3   |
| cell4   | ce
ll5   | cell6   |
|-----------------------------|
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|=============================|
| Foot1   | Foot2   | Foot3   |

## 定义列表

定义列表标题
：定义列表划分。

初创公司
：初创公司或创业公司是指旨在寻求可重复、可扩展商业模式的公司或临时组织。

#dowork
：由 Rob Dyrdek 和他的私人保镖 Christopher “Big Black” Boykins 创造，“Do Work” 可以作为一种自我激励，也可以激励你的朋友

Do It Live
：让[Bill O'Reilly](https://www.youtube.com/watch?v=O_HyZ5aW76c “We'll Do It Live”) 来解释一下

## 无序列表（嵌套）

* 列表项一
    * 列表项一
      * 列表项一
      * 列表项二
      * 列表项三
      * 列表项四
    * 列表项二
    * 列表项三
    * 列表项四
* 列表项二
* 列表项三
* 列表项四

## 有序列表（嵌套）

1. 列表项一
    1. 列表项一
        1. 列表项一
        2. 列表项二
        3. 列表项三
        4. 列表项四
    2. 列表项二
    3. 列表项三
    4. 列表项四
2. 列表项二
3. 列表项三
4. 列表项四



## 按钮

使用 `.btn` 类可以使任何链接更加突出。

## 通知

使用以下语法来提醒：

```markdown
**注意！** 您还可以通过在段落后一行添加`{: .notice}` 来添加提醒  
{: .notice}
```
渲染结果如下：

**注意！** 您还可以通过在段落后一行添加`{: .notice}`来添加提醒
{: .notice}
### Footnotes

Footnotes can be useful for clarifying points in the text, or citing information.[^1] Markdown support numeric footnotes, as well as text as long as the values are unique.[^note]

```markdown
This is the regular text.[^1] This is more regular text.[^note]

[^1]: This is the footnote itself.
[^note]: This is another footnote.
```

[^1]: Such as this footnote.
[^note]: When using text for footnotes markers, no spaces are permitted in the name.

## HTML Tags

### Address Tag

<address>
  1 Infinite Loop<br /> Cupertino, CA 95014<br /> United States
</address>

### Anchor Tag (aka. Link)

This is an example of a [link](http://github.com "Github").

### Abbreviation Tag

The abbreviation CSS stands for "Cascading Style Sheets".

*[CSS]: Cascading Style Sheets

### Cite Tag

"Code is poetry." ---<cite>Automattic</cite>

### Code Tag

You will learn later on in these tests that `word-wrap: break-word;` will be your best friend.

You can also write larger blocks of code with syntax highlighting supported for some languages, such as Python:

```python
print('Hello World!')
```

or R:

```R
print("Hello World!", quote = FALSE)
```

### 删除标签

此标签允许您<strike>删除文本</strike>。

### 强调标签

强调标签应使文本变为斜体。

### 插入标签

此标签应指示<ins>插入</ins>文本。

### 键盘标签

这个鲜为人知的标签模拟了<kbd>键盘文本</kbd>，其样式通常类似于`<code>`标签。

### Preformatted Tag

This tag styles large blocks of code.

<pre>
.post-title {
  margin: 0 0 5px;
  font-weight: bold;
  font-size: 38px;
  line-height: 1.2;
  and here's a line of some really, really, really, really long text, just to see how the PRE tag handles it and to find out how it overflows;
}
</pre>

### 引用标签

<q>开发者，开发者，开发者——</q> ——史蒂夫·鲍尔默

### 强标签

此标签显示**粗体文本**。

### 下标标签

使用H<sub>2</sub>O进行科学样式设计，它会将“2”向下推。

### 上标标签

E= MC<sup>2</sup>，这会将“2”向上推。

### 变量标签

这允许您表示<var>变量</var>。

***
**Footnotes**

The footnotes in the page will be returned following this line, return to the section on <a href="#footnotes">Markdown Footnotes</a>.

