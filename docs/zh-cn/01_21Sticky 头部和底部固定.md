# <b> 头部和底部固定</b>

[效果页面](../assets/source/01_21头部和底部固定.html ':include :type=iframe width=100% height=300px')

[:point_right: 在 codepen 上编辑代码](https://codepen.io/shuangcs/pen/GxbZzv)

![标签](../assets/html.svg)

```html
<div class="wrap flex flex-v">
        <div class="header">我想要它固定顶部部</div>
          <div class="main flex-1">
            <p>呀，自动适应高度，滚上去了</p>
            <p>呀，自动适应高度，滚上去了</p>
            <p>呀，自动适应高度，滚上去了</p>
            <p>呀，自动适应高度，滚上去了</p>
            <p>呀，自动适应高度，滚上去了</p>
            <p>呀，自动适应高度，滚上去了</p>
            <p>呀，自动适应高度，滚上去了</p>
            <p>呀，自动适应高度，滚上去了</p>
            <p>呀，自动适应高度，滚上去了</p>
            <p>呀，自动适应高度，滚上去了</p>
            <p>呀，自动适应高度，滚上去了</p>
            <p>呀，自动适应高度，滚上去了</p>
            <p>呀，自动适应高度，滚上去了</p>
          </div>
        <div class="footer">我想要它固定底部</div>
      </div>
```

![标签](../assets/css.svg)

```css
html,
body {
  height: 100%;
}
.wrap {
  width: 100%;
  height: 100%;
}
.flex {
  display: -webkit-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
}
.flex-v {
  -webkit-box-orient: vertical;
  -webkit-flex-direction: column;
  -ms-flex-direction: column;
  flex-direction: column;
}

.header,
.footer {
  height: 40px;
  line-height: 40px;
  background-color: beige;
}
.main {
  overflow: auto;
  -webkit-overflow-scrolling: touch;
  padding: 10px;
  line-height: 1.5;
}

.flex-1 {
  -webkit-box-flex: 1;
  -webkit-flex: 1;
  -ms-flex: 1;
  flex: 1;
}
```
