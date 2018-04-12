# <b>Sticky Header 头部固定</b>

> header 固定在顶部，不会随着页面滚动

[效果页面](../assets/source/01flex-头部固定.html ':include :type=iframe width=100% height=483px')

[:point_right: 在codepen上编辑代码](https://codepen.io/shuangcs/pen/PRLjXP)

![标签](../assets/html.svg)

```html
<header>头部</header>
<article>主要内容</article>
<footer>底部</footer>
```

![标签](../assets/css.svg)

```css
 body{
    height: 100vh;
    display: flex;
    flex-direction: column;
    padding-top: 60px;
    margin: 0;
}
header {
    height: 60px;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    padding: 0;
    background-color:beige;
}
article {
    flex: auto;
    height: auto;
    background: mediumaquamarine;
}
footer {
    height: 70px;
    background-color:beige;
}
```