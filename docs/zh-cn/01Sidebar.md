# <b> Sidebar 侧边栏</b>

> 左边是定宽 sidebar，右边是上-中-下布局。

[效果页面](00flex03.html ':include :type=iframe width=100% height=600px')

[:point_right: 在codepen上编辑代码](https://codepen.io/shuangcs/pen/BrbZGK)

![标签](../assets/html.svg)

```html
<aside>左侧</aside> 
<div class="content"> 
  <header>头部</header> 
  <article>主要内容</article> 
  <footer>底部</footer> 
</div> 
```

![标签](../assets/css.svg)

```css
body { 
  min-height: 100vh; 
  display: flex; 
} 
 
aside { 
  flex: none; 
  width: 200px;
  background-color: beige;
} 
 
.content { 
  flex: auto; 
  display: flex; 
  flex-direction: column; 
 
} 
 
.content article { 
  flex: auto;
  background: mediumaquamarine;
} 
.content header {
  background-color: beige;
}
.content header {
  height: 50px;
  background-color: beige;
}
.content footer {
  height: 50px;
  background-color: beige;
}
```