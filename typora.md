# Typora 笔记

## 常用快捷键

| 快捷键              | 场景   | 作用         |
| ---------------- | ---- | ---------- |
| Ctrl+Shift+V     |      | 粘贴成文本      |
| Shift+Return     |      | `<br/`     |
| **Shift+Return** | 表格   | 在当前行后面插入一行 |
| Ctrl+\           |      | 清除格式       |

## 智能操作

| 输入              | 场景   | 操作     |
| --------------- | ---- | ------ |
| `标题1标题2`     |      | 创建表格   |
| `[toc]` `Enter` |      | 创建目录   |
| `***` 或  `---`  |      | 横线     |
| `---`           | 开头   | YAML 头 |

## 行内元素

### 示例

```markdown
* 链接： [Wikipedia](http://wikipedia.org, "维基百科")
* 图片： ![维基百科](https://www.wikipedia.org/portal/wikipedia.org/assets/img/Wikipedia-logo-v2.png)
* 强调： *强调*
* 粗体： **粗体**
* 代码： `print()`
* 删除线： ~~我错了~~
* 下划线： __这样不行__，<u>要这样</u>
* Emoji 表情： :smile:
* 高亮：==highlight==，不通用
```

### 效果

* 链接： [Wikipedia](http://wikipedia.org, "维基百科")
* 图片：![维基百科](https://www.wikipedia.org/portal/wikipedia.org/assets/img/Wikipedia-logo-v2.png)
* 强调： *强调*
* 粗体： **粗体**
* 代码： `print()`
* 删除线： ~~我错了~~
* 下划线： __这样不行__，<u>要这样</u>
* Emoji 表情： :smile:
* 高亮：==highlight==，不通用

##  块级元素

### 标题

```markdown
# 标题1
## 标题2
###### 标题6
```

### 目录（TOC)

输入 `[toc]` 然后 `Enter`。

### 表格

输入 `| 标题1 | 标题2 |`然后按`Enter`。

`Shift+Enter` 添加一行。

### 块引用

示例：

```markdown
> 包含两段的引用，这是段落1
>
> 段落2

> 另一个引用。
```

### 列表

```## un-ordered list*   Red*   Green*   Blue## ordered list1.  Red2. 	Green3.	Blue

### 任务列表

​```markdown
- [ ] a task list item
- [ ] list syntax required
- [ ] normal **formatting**, @mentions, #1234 refs
- [ ] incomplete
- [x] completed
```

### 代码块

```gfm
示例:
​```
function test() {
  console.log("notice the blank line before this function?");
}
​```

语法高亮:
​```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
​```
```

### 脚注

```markdown
创建脚注的方法[^脚注]

[^脚注]: **脚注**的*内容*。
```

效果如下：

创建脚注的方法[^脚注]

[^脚注]: **脚注**的*内容*。

### 其他

#### 数学公式

（略）

#### 横线

`***` 或 `---`

#### YAML 头

Typora 支持 [YAML Front Matters](http://jekyllrb.com/docs/frontmatter/)。

在文章开头输入 `---` 然后 `Enter` 即可。

#### 绘图

参见 [用 Markdown 绘图](http://support.typora.io/Draw-Diagrams-With-Markdown/) 。
