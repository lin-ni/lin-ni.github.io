这是一篇自用笔记，记载着 Markdown + docsify 自定义功能/插件的使用方式。

---

## 文字

<!-- tabs:start -->

#### ** 效果 **

文字

**粗体**

_斜体_

~~删除线~~

<mark>加亮文字</mark>

<pre>Preformatted text - 无格式文字</pre>

<small>小字</small>

这是 <sub>下标</sub>

这是 <sup>上标</sup>

#### ** Markdown **

```
文字

**粗体**

*斜体*

~~删除线~~

<mark>加亮文字</mark>

<pre>Preformatted text - 无格式文字</pre>

<small>小字</small>

这是 <sub>下标</sub>

这是 <sup>上标</sup>
```

<!-- tabs:end -->

## 强调内容

`> 这是一段引用内容。`

> 这是一段引用内容。

`!> 这是一段强调内容。`

!> 这是一段强调内容。

`?> 这是一段信息内容。`

?> 这是一段信息内容。

## 标签页

<!-- tabs:start -->

#### ** 效果 **

如此可见

#### ** Markdown **

```
<!-- tabs:start -->

#### ** 标签页A **

标签页A详细内容。

#### ** 标签页B **

标签页B详细内容。

<!-- tabs:end -->
```

<!-- tabs:end -->

## 选项框下拉

### 单项选择

<!-- tabs:start -->

#### ** 效果 **

<!-- select:start -->
<!-- select-menu-labels: 标题 -->

这是一段介绍。

#### --选项 A--

选项 A 显示的文字。

#### --选项 B--

选项 B 显示的文字。

<!-- select:end -->

#### ** Markdown **

```
<!-- select:start -->
<!-- select-menu-labels: 标题 -->

这是一段介绍。

#### --选项A--

选项A显示的文字。

#### --选项B--

选项B显示的文字。

<!-- select:end -->
```

<!-- tabs:end -->

### 双项选择

<!-- select:start -->
<!-- select-menu-labels: 标题A,标题B -->

这是一段介绍。

### --选项 A,选项 a--

选项 A + 选项 a

### --选项 B,选项 a--

选项 B + 选项 a

### --选项 C,选项 a--

选项 C + 选项 a

### --选项 A,选项 b--

选项 A + 选项 b

### --选项 B,选项 b--

选项 B + 选项 b

### --选项 C,选项 b--

选项 C + 选项 b

<!-- select:end -->

#### Markdown

```
<!-- select:start -->
<!-- select-menu-labels: 标题A,标题B -->

这是一段介绍。

### --选项A,选项a--

选项A + 选项a

### --选项B,选项a--

选项B + 选项a

### --选项C,选项a--

选项C + 选项a

### --选项A,选项b--

选项A + 选项b

### --选项B,选项b--

选项B + 选项b

### --选项C,选项b--

选项C + 选项b

<!-- select:end -->
```

## HTML 标签中的 Markdown

<!-- tabs:start -->

#### ** 效果 **

<details>
<summary>自我评价（点击展开）</summary>

- Abc
- Abc

</details>

#### ** Markdown **

```
<details>
<summary>自我评价（点击展开）</summary>

- Abc
- Abc

</details>
```

<!-- tabs:end -->
