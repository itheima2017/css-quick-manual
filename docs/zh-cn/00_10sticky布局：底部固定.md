# <b>sticky布局：底部固定</b>

[效果页面](../assets/source/00布局-底部固定.html ':include :type=iframe width=100% height=323px')

[:point_right: 在codepen上编辑代码](https://codepen.io/shuangcs/pen/JLBvEL)

![标签](../assets/html.svg)

```html
<div class="content">
    <div class="wrapper">
        <div class="title">
            <p>这里是头部</p>
        </div>
        <div class="main">
            <p>这里是main content区域...</p>
            <p>这里是main content区域...</p>
            <p>这里是main content区域...</p>
            <p>这里是main content区域...</p>
        </div>
    </div>
</div>
<div class="footer">
    <p>底部固定</p>
</div>
```

![标签](../assets/css.svg)

```css
* {
    margin: 0;
    padding: 0;
}
.title {
    height: 64px;
    line-height: 64px;
    background-color: bisque;
}
html,
body,
.content {
    height: 100%;
    text-align: center;
}

body>.content {
    height: 100%;
    min-height: 100%;
}

.main {
    padding-bottom: 64px; 
}

.footer {
    position: relative;
    margin-top: -64px;  
    height: 64px;      
    text-align: center;
    line-height: 64px;
    clear: both;
    background-color: bisque;
}
```
<b>说明</b>
1. footer要与其他所有内容在同一级别；
2. 若要添加其它同级层，那这个同级层就必须使用position:absolute进行绝对定位；

