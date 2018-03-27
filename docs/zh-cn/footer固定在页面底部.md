# <b>footer固定在页面底部</b>

![效果](./../assets/footer1.png)

##### <b>方案一：Sticky footer布局 — 负 margin 方式</b>

`HTML`

```html
<div class="content">
    <div class="wrapper">
        <div class="title">
            <h1>这里是头部</h1>
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
    <p>© 2018 No rights reserved.</p>
    <p>Made with ♥ by an anonymous pastafarian.</p>
</div>
```

`CSS`
```css
* {
    margin: 0;
    padding: 0;
}

html,
body,
.content {
    height: 100%;
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
    clear: both;
    background-color: red;
}
```
<b>说明</b>
1. footer要与其他所有内容在同一级别；
2. 若要添加其它同级层，那这个同级层就必须使用position:absolute进行绝对定位；

##### <b>方案二：Sticky footer布局 — flex 方式</b>

`HTML`
```html
<header> 
    <h1>这里是头部</h1> 
</header> 
<div class="main"> 
    <p>这里是main content区域...</p> 
    <p>这里是main content区域...</p>
    <p>这里是main content区域...</p>
    <p>这里是main content区域...</p>
</div> 
<footer> 
    <p>© 2018 No rights reserved.</p> 
    <p>Made with ♥ by an anonymous pastafarian.</p> 
</footer>
```

```css
* {
    margin: 0;
    padding: 0;
}

body {
    display: flex;
    flex-flow: column;
    min-height: 100vh;
    overflow: auto;
}

h1 {
    font-size: 60px;
    text-align: center;
}

p {
    font-size: 24px;
    text-align: center;
}

.main {
    flex: 1;
}
footer {
    background-color: red;
}
```
<b>浏览器支持</b>
<iframe src="https://caniuse.bitsofco.de/embed/index.html?feat=flexbox&amp;periods=future_2,future_1,current,past_1,past_2,past_3&amp;accessible-colours=false" frameborder="0" width="100%" height="510px"></iframe>

