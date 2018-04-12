# <b> Sticky Sidebar 左侧栏固定</b>

> 左侧 sidebar 固定在左侧且与视窗同高，当内容超出视窗高度时，在 sidebar 内部出现滚动条。左右两侧滚动条互相独立。

[效果页面](00flex05.html ':include :type=iframe width=100% height=580px')

[:point_right: 在codepen上编辑代码](https://codepen.io/shuangcs/pen/LdaLMq)

![标签](../assets/html.svg)

```html
<aside>
    <h3>左侧列表</h3>
    <p>选项一</p>
    <p>选项一</p>
    <p>选项一</p>
    <p>选项一</p>
</aside>
<div class="content">
    <header>头部</header>
    <article>内容区</article>
    <footer>底部</footer>
</div>
```

![标签](../assets/css.svg)

```css
aside {
    flex:none;
    width: 200px;
    overflow-y: auto;
    display: block;
    background: bisque;
}
.content {
    flex: auto;
    display: flex;
    flex-direction: column;
    overflow-y: auto;
}
.content header {
    height: 70px;
    background-color: beige;
}
.content article {
    flex: auto;
    background: mediumaquamarine;
}
.content footer {
    height: 100px;
    background-color: beige;
}
```