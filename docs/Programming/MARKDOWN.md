

# Markdown 语法手册 {#main}

##### *TAG :* `Markdown` `HTML`

[<目录>](#main)
* [A. 样式](#style)
    - [1. 斜体](#style_1)
    - [2. 粗体](#style_2)
    - [3. 删除线](#style_3)
* [B. 格式](#format)
    - [1. 标题](#format_1)
    - [2. 标签](#format_2)
    - [3. 段落](#format_3)
* [C. 列表](#list)
    - [1. 无序列表](#list_1)
    - [2. 有序列表](#list_2)
* [D. 链接 & 图片](#link)
    - [1. 链接](#link_1)
    - [2. 图片](#link_2)
* [E. 引用 & 代码](#code)
    - [1. 引用](#code_1)
    - [2. 注脚](#code_2)
    - [3. 行内代码块](#code_3)
    - [4. 代码块](#code_4)
* [F. 表格](#table)
    - [1. 基础表格](#table_1)
    - [2. HTML标签](#table_2)

---

## A. 样式 {#style}

### 1. 斜体 (italic) {#style_1}

使用 `*`或`_` 表示**斜体**，可混用。
```
这是 *斜体*，这也是 _斜体_。
```
> 这是 *斜体*，这也是 _斜体_。

### 2. 粗体 (bold) {#style_2}

使用 `**`或`__` 表示**粗体**，可混用。
```
这是 *粗体*，这也是**粗体**。
```
> 这是 **粗体**，这也是__粗体__。

### 3. 删除线 (cross-out) {#style_3}

使用`~~`表示**删除线**。

`~~划掉此处~~`

> ~~划掉此处~~

###### [Back](#main)
---

## B. 格式 {#format}

### 1. 标题 (heading) {#format_1}

使用 `===` 表示**一级标题**，使用 `---` 表示**二级标题**。

使用 `#{n}`表示 *不同级别* 的标题 (H1-H6)，例如：### H3。

也可使用`#{n}  #{n}`表示，例如：### H3 ###。


```
一级标题 <h1>
============================

二级标题 <h2>
--------------------------------------------------

### 三级标题 <h3>
#### 四级标题 <h4> ####
```

> 一级标题 <h1>
> ============================
> 
> 二级标题 <h2>
> --------------------------------------------------
> 
> ### 三级标题 <h3>
> #### 四级标题 <h4> ####

### 2. 标签 (tag) {#format_2}

使用`{#id}`为标题添加定位**id**标签。

```
## 正文 {#main}
```

> ## 正文 {#main}

### 3. 段落 (paragraph) {#format_3}

每段段落中间空一行或多行，否则视为同一段落。

###### [Back](#main)
---

## C. 列表 {#list}

### 1. 无序列表 (unordered list) {#list_1}

使用 `*`或`+`或`-` 表示**无序列表**， 多层缩进表示子列表。

```
- 无序列表项 一
    - 子列表
+ 无序列表项 二
* 无序列表项 三
```

> - 无序列表项 一
>   - 子列表
> + 无序列表项 二
> * 无序列表项 三

### 2. 有序列表 (ordered list) {#list_2}

使用`n.`表示**有序列表**，列表*自动编号*，多层缩进表示子列表。
```
1. 有序列表项 一
    1. 子列表
3. 有序列表项 二
7. 有序列表项 三
```
> 1. 有序列表项 一
>     1. 子列表
> 2. 有序列表项 二
> 3. 有序列表项 三

###### [Back](#main)
---

## D. 链接 & 图片 {#link}

### 1. 外链接 (link) {#link_1}

使用 `[描述](URL)` 为文字增加**外链接**，链接可以是 *相对链接* ／ *绝对链接* ／ *标签*。
```
[我是链接](https://littleb-order.github.io/sharing/)
```
[我是链接](https://littleb-order.github.io/sharing/)


### 2. 插入图像 (image) {#link_2}

使用 `![描述](图片链接)` 插入图像。

    ![图片](http://via.placeholder.com/36x36.jpg)

> ![图片](http://via.placeholder.com/36x36.jpg)

###### [Back](#main)
---

## E. 引用 & 代码 {#code}

### 1. 文字引用 (quote) {#code_1}

使用 `>` 表示**文字引用**, 空一行取消格式。
```
> 引用的文字 
>> 重复引用的文字。
```
> 引用的文字 
>> 重复引用的文字。

### 2. 注脚 (footnote) {#code_2}

使用 `[^关键词]` 表示注脚，以及`[^关键词]:注释内容`表示注释内容。

```
有关**数据**[^注]显示

[^注]: 数据截止自2012年12月31日
```

> 有关**数据**[^注]显示
>
> [^注]: 数据截止自2012年12月31日

### 3. 行内代码块 (inline) {#code_3}

使用 `` `code` `` 表示** *行内* 代码块**, 空一行取消格式。

`<html></html>`

> `<html></html>`

### 4.  代码块 (block) {#code_4}

- 使用`四个缩进空格`表示**代码块**。

```
    <=四个缩进空格 代码
```

>    <=四个缩进空格 代码


- 使用` ```编程语言 `和` ``` `显示**支持高亮**的代码。

```
``` javascript
// A sample javascript code
function bar(){
    console.log('Hello World.');
}
```

> ``` javascript
> // A sample javascript code
> function bar(){
>     console.log('Hello World.');
> }
> ```

###### [Back](#main)
---

## F. 表格 {#table}

### 1. 基本表格 {#table_1}

```
|   标题  |   标题  |   标题  |
|   ---  |  :---:  |   ---: |
| 居左    |   居中  |   居右  |
| 单元格   |   单元格 |   单元格 |
```

> |   标题  |   标题  |   标题  |
> |   ---  |  :---:  |   ---: |
> | 居左    |   居中  |   居右  |
> | 单元格   |   单元格 |   单元格 |

### 2. HTML标签 {#table_2}

可使用**HTML标签**嵌套在Markdown语法中创建复杂表格。

    <table>
        <tr>
            <th rowspan="2">表格</th>
            <th align="left">居左</th>
            <th align="center">居中</th>
            <th align="right">居右</th>
        </tr>
        <tr>
            <td>单元格</td>
            <td>单元格</td>
            <td>单元格</td>
        </tr>
    </table>


<table>
    <tr>
        <th rowspan="2">表格</th>
        <th align="left">居左</th>
        <th align="center">居中</th>
        <th align="right">居右</th>
    </tr>
    <tr>
        <td>单元格</td>
        <td>单元格</td>
        <td>单元格</td>
    </tr>
</table>

###### [Back](#main)
---
