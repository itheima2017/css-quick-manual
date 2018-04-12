# <b>Sticky Footer 底部固定</b>

> 当页面内容高度小于可视区域高度时，footer 吸附在底部；当页面内容高度大于可视区域高度时，footer 被撑开排在 content 下方。

[效果页面](../assets/source/01flex-底部固定.html ':include :type=iframe width=100% height=483px')

[:point_right: 在codepen上编辑代码](https://codepen.io/shuangcs/pen/EEMXeR)

![标签](../assets/html.svg)

```html
<header>头部</header>
<article>主要内容</article>
<footer>底部</footer>
```

![标签](../assets/css.svg)

```css
body { 
    min-height: 100vh; 
    display: flex; 
    flex-direction: column; 
    padding: 0;
    margin: 0
} 
header {
    height: 70px;
    background: bisque;
}
article { 
    flex: auto;
    background: mediumaquamarine;
} 
footer {
    height: 70px;
    background: bisque;
}
```