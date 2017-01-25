---
title: Cmd Markdown 简明语法手册（删减）
date: 2016-10-12 19:22:33
tags: markdown
description: markdown文本编辑利器，简明语法手册，依据个人喜好有所修改，增加示例对比
toc: true
categories: add
comments: true
mathjax: true
---
------

## Cmd Markdown 简明语法手册（删减）

### 1. 斜体和粗体

使用 * 和 ** 表示斜体和粗体。
示例：

    这是 *斜体*，这是 **粗体**。

效果：这是 *斜体*，这是 **粗体**。

斜体快捷键：（快捷键ctrl+i），粗体快捷键：（快捷键ctrl+b）



### 2. 分级标题

示例：

    # 这是一个一级标题
    
    ## 这是一个二级标题
    
    ### 这是一个三级标题

效果：
# 这是一个一级标题
## 这是一个二级标题
### 这是一个三级标题

----------

### 3. 外链接

使用 \[描述](链接地址) 为文字增加外链接。

示例：

    这是去往[本人博客](http://stephenxtech.com)的链接

效果：
这是去往[本人博客](http://stephenxtech.com)的链接
### 4. 无序列表

使用 *，+，- 表示无序列表。

示例：

    （首行留空，否则无效果）    
     - 列表项
     - 无序列表项 一
     - 无序列表项 二
     - 无序列表项 三
效果：
- 列表项
- 无序列表项 一
- 无序列表项 二
- 无序列表项 三
### 5. 有序列表

使用数字和点表示有序列表。

示例：

1. 有序列表项 一
2. 有序列表项 二
3. 有序列表项 三

### 6. 文字引用

使用 > 表示文字引用。

示例：

> 野火烧不尽，春风吹又生
    
效果：
> 野火烧不尽，春风吹又生

### 7. 行内代码块

使用 \`代码` 表示行内代码块。

示例：

    让我们聊聊 `html`。
效果：
让我们聊聊 `html`。
### 8.  代码块

使用 四个缩进空格 表示代码块。

示例：
这是一个代码块，此行左侧有四个不可见的空格。
效果：

    这是一个代码块，此行左侧有四个不可见的空格。

### 9.  插入图像

使用 \!\[描述](图片链接地址) 插入图像。

示例：

    ![我的头像](https://www.zybuluo.com/static/img/my_head.jpg)

效果：
![我的头像](https://www.zybuluo.com/static/img/my_head.jpg)

# Cmd Markdown 高阶语法手册

### 1. 内容目录

在段落中填写 `[TOC]` 以显示全文内容的目录结构。
效果：

[TOC]

### 3. 删除线
~~删除线好有意思啊~~
使用 ~~ 表示删除线。
示例：

    ~~这是一段错误的文本。~~

效果：
~~这是一段错误的文本。~~

### 5. LaTeX 公式

表示行内公式： 
示例
    
    质能守恒方程可以用一个很简洁的方程式 $E=mc^2$ 来表达。
效果：
质能守恒方程可以用一个很简洁的方程式 $E=mc^2$ 来表达。

表示整行公式：
    
    $$\sum_{i=1}^n a_i=0$$
    
    $$f(x_1,x_x,\ldots,x_n) = x_1^2 + x_2^2 + \cdots + x_n^2 $$
    
    $$\sum^{j-1}_{k=0}{\widehat{\gamma}_{kj} z_k}$$
效果：
$$\sum_{i=1}^n a_i=0$$
$$f(x_1,x_x,\ldots,x_n) = x_1^2 + x_2^2 + \cdots + x_n^2 $$
$$\sum^{j-1}_{k=0}{\widehat{\gamma}_{kj} z_k}$$

访问 [MathJax](http://meta.math.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference) 参考更多使用方法。

### 6. 加强的代码块

支持四十一种编程语言的语法高亮的显示，行号显示。

非代码示例：

    ```
    $ sudo apt-get install vim-gnome
    ```
效果：
```
$ sudo apt-get install vim-gnome
```
Python 示例：

    ```python
    @requires_authorization
    def somefunc(param1='', param2=0):
        '''A docstring'''
        if param1 > param2: # interesting
            print 'Greater'
        return (param2 - param1 + 1) or None
    
    class SomeClass:
        pass
    
    >>> message = '''interpreter
    ... prompt'''
    ```
效果：
```python
@requires_authorization
def somefunc(param1='', param2=0):
    '''A docstring'''
    if param1 > param2: # interesting
        print 'Greater'
    return (param2 - param1 + 1) or None
class SomeClass:
    pass
>>> message = '''interpreter
... prompt'''
```


### 12. 表格支持
示例：
    | 项目        | 价格   |  数量  |
    | --------   | -----:  | :----:  |
    | 计算机     | \$1600 |   5     |
    | 手机        |   \$12   |   12   |
    | 管线        |    \$1    |  234  |

效果：
| 项目        | 价格   |  数量  |
| --------   | -----:  | :----:  |
| 计算机     | \$1600 |   5     |
| 手机        |   \$12   |   12   |
| 管线        |    \$1    |  234  |



### 15. 内嵌图标

本站的图标系统对外开放，在文档中输入

    <i class="icon-weibo"></i>

即显示微博的图标： <i class="icon-weibo icon-2x"></i>

替换 上述 `i 标签` 内的 `icon-weibo` 以显示不同的图标，例如：

    <i class="icon-renren"></i>

即显示人人的图标： <i class="icon-renren icon-2x"></i>

更多的图标和玩法可以参看 [font-awesome](http://fortawesome.github.io/Font-Awesome/3.2.1/icons/) 官方网站。

### 16. 待办事宜 Todo 列表

使用带有 [ ] 或 [x] （未完成或已完成）项的列表语法撰写一个待办事宜列表，并且支持子列表嵌套以及混用Markdown语法，例如：

    - [ ] **Cmd Markdown 开发**
        - [ ] 改进 Cmd 渲染算法，使用局部渲染技术提高渲染效率
        - [ ] 支持以 PDF 格式导出文稿
        - [x] 新增Todo列表功能 [语法参考](https://github.com/blog/1375-task-lists-in-gfm-issues-pulls-comments)
        - [x] 改进 LaTex 功能
            - [x] 修复 LaTex 公式渲染问题
            - [x] 新增 LaTex 公式编号功能 [语法参考](http://docs.mathjax.org/en/latest/tex.html#tex-eq-numbers)
    - [ ] **七月旅行准备**
        - [ ] 准备邮轮上需要携带的物品
        - [ ] 浏览日本免税店的物品
        - [x] 购买蓝宝石公主号七月一日的船票
        
对应显示如下待办事宜 Todo 列表：
        
- [ ] **Cmd Markdown 开发**
    - [ ] 改进 Cmd 渲染算法，使用局部渲染技术提高渲染效率
    - [ ] 支持以 PDF 格式导出文稿
    - [x] 新增Todo列表功能 [语法参考](https://github.com/blog/1375-task-lists-in-gfm-issues-pulls-comments)
    - [x] 改进 LaTex 功能
        - [x] 修复 LaTex 公式渲染问题
        - [x] 新增 LaTex 公式编号功能 [语法参考](http://docs.mathjax.org/en/latest/tex.html#tex-eq-numbers)
- [ ] **七月旅行准备**
    - [ ] 准备邮轮上需要携带的物品
    - [ ] 浏览日本免税店的物品
    - [x] 购买蓝宝石公主号七月一日的船票
        
PS：以上修改自作业部落[Cmd Markdown 简明语法手册](http://docs.mathjax.org/en/latest/tex.html#tex-eq-numbers)，仅个人记录喜好
