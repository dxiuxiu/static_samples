# css 文本属性

+ 文本转换(text-transform)
+ 字间隔 word-spacing 与字母间隔 letter-spacing
+ 文本阴影 text-shadow
+ word-wrap（overflow-wrap
+ white-space、word-wrap、word-break

## 常用

+ 文字单行/多行超出隐藏
+ 文字两端对齐

## 其它

### 文本转换(text-transform)

```css
p{
    text-transform:none|capitalize|uppercase|lowercase|inherit
}
```

+ none 默认。定义带有小写字母和大写字母的标准的文本。
+ capitalize 文本中的每个单词以大写字母开头。
+ uppercase 定义仅有大写字母。
+ lowercase 定义无大写字母，仅有小写字母。
+ inherit 规定应该从父元素继承 text-transform 属性的值。

### word-wrap（overflow-wrap）

> 注：word-wrap 属性原本属于微软的一个私有属性，在 CSS3 现在的文本规范草案中已经被重名为 overflow-wrap 。 word-wrap 现在被当作 overflow-wrap 的 “别名”。 稳定的谷歌 Chrome 和 Opera 浏览器版本支持这种新语法。

### white-space、word-wrap、word-break

+ white-space 如何处理元素内空白
+ word-wrap 是否允许浏览器在单词内进行断句
+ word-break 怎么样进行单词内的断句

```css
p{
    white-space: pre-wrap;
    word-wrap:break-word;
    word-break:break-all;
}
```

#### white-space

+ normal 默认。空白会被浏览器忽略。
+ pre 空白会被浏览器保留。其行为方式类似 HTML 中的 pre 标签。
+ nowrap文本不会换行，文本会在在同一行上继续，直到遇到 br 标签为止。
+ pre-wrap 保留空白符序列，但是正常地进行换行。
+ pre-line 合并空白符序列，但是保留换行符。
+ inherit 规定应该从父元素继承 white-space 属性的值。

#### word-wrap（overflow-wrap）

+ normal: 只在允许的断字点换行(浏览器保持默认处理)
+ break-word:在长单词或URL地址内部进行换行，
/*内容将在边界内换行。如果需要，单词内部允许断行。*/

#### word-break

+ normal：使用浏览器默认的换行规则。
+ break-all:允许在单词内换行 ， 允许任意非CJK(Chinese/Japanese/Korean)文本间的单词断行。
+ keep-all:只能在半角空格或连字符处换行，
