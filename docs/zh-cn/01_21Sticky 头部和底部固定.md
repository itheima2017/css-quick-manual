# <b> 头部和底部固定</b>

[效果页面](../assets/source/01_21头部和底部固定.html ':include :type=iframe width=100% height=600px')

[:point_right: 在codepen上编辑代码](https://codepen.io/shuangcs/pen/GxbZzv)

![标签](../assets/html.svg)
```html
<header>头部</header>
<article>
  <p>呀，被滚到上面去了</p>
  <p>呀，被滚到上面去了</p>
  <p>呀，被滚到上面去了</p>
  <p>呀，被滚到上面去了</p>
</article>
<footer>底部</footer>
```
![标签](../assets/css.svg)

```css
body {
  height: 100vh;
  display: flex;
  flex-direction: column;
  padding-top: 40px;
  margin: 0;
}

header {
  height: 40px;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  padding: 0;
  background-color: beige;
}

article {
  flex: auto;
  height: auto;
  background: mediumaquamarine;
}

footer {
  height: 50px;
  background-color: beige;
  position: fixed;
  bottom: 0;
  width: 100%;
}
```