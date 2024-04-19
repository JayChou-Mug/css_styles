# Typora 自定义样式

## 代码块

```css
/* 代码块样式 */
/* 设置整体 */
.md-fences {
  background-color: #f8f8f8;
  border-radius: 5px;
  box-shadow: 0 10px 30px 0 rgb(0 0 0 / 40%);
  padding-top: 30px;
  font-family: monospace, 'PingFang SC', 'Microsoft YaHei';
}
 
/* 设置三个圈圈 */
.md-fences::before {
  background: #fc625d;
  border-radius: 50%;
  box-shadow: 20px 0 #fdbc40, 40px 0 #35cd4b;
  content: ' ';
  height: 12px;
  left: 12px;
  margin-top: -20px;
  position: absolute;
  width: 12px;
}
```

**代码块字体主题色**

### 函数调用

```python
A = np.arange(12).reshape(3,4) 
```

```css
.cm-s-inner .cm-property {
    color: #f5ad32;
}
```

### 数字

```python
a = 1 + 2
```

```css
.cm-s-inner .cm-number {
    color: rgb(19, 137, 240);
}
```

### 内置函数

```python
map() print() id() filter()
```

```css
.cm-s-inner .cm-builtin {
    color: #d63200;
}
```

### 基本运算符

```python
> < = ! + - * /
```

```css
.cm-s-inner .cm-operator {
    color: #9c2ff6;
}
```

### 预保留关键字

```python
True False return for in while import
```

```css
.cm-s-inner .cm-keyword {
    color: #e53f73;
}
```

### 注释

```python
# 单行注释 
```

```css
.cm-s-inner .cm-comment,
.cm-s-inner.cm-comment {
    color: #109945;
}
```



## 引用块

```css
blockquote {
  color: #304455;
  border-radius: 2px;
  padding: 10px 16px;
  background-color: #fdefee;
  position: relative;
  border-left: none;
}
 
blockquote:before {
  display: block;
  position: absolute;
  content: '';
  width: 4px;
  left: 0;
  top: 0;
  height: 100%;
  background-color: #e95f59;
  border-radius: 2px;
}
```

## 标题

```css
h1 {
    font-size: 2.5em;
    text-align: center;
}
```



## 加粗

```css
strong {
  font-size: 20px;
  color: #e95f59;
}
```

## 高亮

```css
mark {
  background: #fdefee;
  color: #e95f59;
  font-size: 18px;
  margin: 0 5px;
  font-weight: bold;
}
```

## 行内代码

```css
code {
  background-color: rgba(66, 185, 131, 0.1);
  padding: 0 2px 0 2px;
  color: #42b983;
}
```

## 图片默认居左

```css
p .md-image:only-child {
  width: auto;
  text-align: left;
}
```

## 字体

均写在css文件中对应代码段的花括号内

###  粗体

```css
font-weight: bold;
```

### 斜体

```css
font-style: italic;
```

### 样式

```css
 font-family: 'Consolas';  /*改为你需要的字体*/
```

### 大小

```css
font-size: 19px;  /*数字改为你需要的大小*/
```

### 颜色

```css
color: #e38f00;  /*支持16进制颜色代码与RGB色彩*/
color: rgb(19, 137, 240);
```


