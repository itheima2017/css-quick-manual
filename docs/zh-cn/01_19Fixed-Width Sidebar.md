# <b> Fixed-Width Sidebar左侧定宽</b>

> 在上-中-下布局的基础上，加了左侧定宽 sidebar。

[效果页面](../assets/source/01flex-侧栏定宽内容区.html ':include :type=iframe width=100% height=600px')

[:point_right: 在codepen上编辑代码](https://codepen.io/shuangcs/pen/EEMXdp)

![标签](../assets/html.svg)

```html
<header>头部</header> 
<div class="content"> 
    <aside>左侧</aside> 
    <article>内容</article> 
</div> 
<footer>底部</footer>
```

![标签](../assets/css.svg)

```css
body { 
  min-height: 100vh; 
  display: flex; 
  flex-direction: column; 
} 
header {
  height: 70px;
  background: bisque;
}
.content { 
  flex: auto; 
  display: flex; 
  background: mediumaquamarine;
} 
.content aside {
  width: 200px;
  background: beige;
}
.content article { 
  flex: auto; 
}
 
footer {
  height: 70px;
  background: bisque;
}
```