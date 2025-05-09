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

Academic Pages使用[kramdown](https://kramdown.gettalong.org/index.html) 进行Markdown渲染，这与GitHub等其他Markdown实现略有不同。除了本指南外，请参阅 [kramdown 语法页面](https://kramdown.gettalong.org/syntax.html)获取完整文档

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
| [alice](#)    | 2023   | 列表中项目的描述                          |
| [alice](#)    | 2024   | 列表中项目的描述                          |
| [arisu](#)     | 2025   | 列表中项目的描述                          |

### 表2

| 标头1 | 标头2 | 标头3 |
|:--------|:-------:|--------:|
| 1   | 2   | 3   |
| 4   | 5   | 6   |
|-----------------------------|
| 7   | 8   | 9   |
| 10   | 11   | 12   |
|=============================|
| Foot1   | Foot2   | Foot3   |

## 定义列表

定义列表标题
：定义列表划分

初创公司
：初创公司或创业公司是指旨在寻求可重复、可扩展商业模式的公司或临时组织

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
### 脚注

脚注可用于阐明文本要点或引用信息。[^1] Markdown 支持数字脚注，以及文本（只要值是唯一的）。[^note]

```markdown
这是常规文本。[^1] 这是更常规的文本[^note]

[^1]：这是脚注本身
[^note]：这是另一个脚注
```

[^1]：例如此脚注
[^note]：使用文本作为脚注标记时，名称中不允许有空格

## HTML 标签

### 地址标签

<address>
1 Infinite Loop<br /> Cupertino, CA 95014<br /> 美国
</address>

### 锚点标签（又称链接）

这是一个 [link](http://github.com "Github") 的示例。

### 缩写标签

CSS 的缩写代表“层叠样式表”。

*[CSS]：层叠样式表

### 引用标签

“代码如诗” ---<cite>Automattic</cite>

### 代码标签

在后面的测试中，你将了解到 `word-wrap: break-word;` 将是你最好的朋友

您还可以编写更大的代码块，并使用某些语言（例如 Python）支持的语法高亮功能：

```python
print('Hello World!')
```

或 R：

```R
print("Hello World!", quote = FALSE)
```

### 删除标签

此标签允许您<strike>删除文本</strike>

### 强调标签

强调标签应使文本变为*斜体*

### 插入标签

此标签应指示<ins>插入</ins>文本

### 键盘标签

这个鲜为人知的标签模拟了<kbd>键盘文本</kbd>，其样式通常类似于`<code>`标签

### 预格式化标签

此标签用于设置大段代码的样式

<pre>
.post-title {
margin: 0 0 5px;
font-weight: bold;
font-size: 38px;
line-height: 1.2;
这里有一行非常非常非常长的文本，只是为了看看 PRE 标签如何处理它并找出它是如何溢出的；
}
</pre>

### 引用标签

<q>开发者，开发者，开发者...</q> ——史蒂夫·鲍尔默

### 强标签

此标签显示**粗体文本**

### 下标标签

使用H<sub>2</sub>O进行科学样式设计，它会将“2”下标

### 上标标签

E= MC<sup>2</sup>，这会将“2”上标

### 变量标签

这允许您表示变量<var>X</var>

***
**脚注**

页面中的脚注将在此行之后返回，返回到 <a href="#footnotes">Markdown 脚注</a> 部分
