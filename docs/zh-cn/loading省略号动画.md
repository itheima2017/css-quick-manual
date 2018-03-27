# <b>loading省略号动画</b>

![效果](./../assets/layout1.png)

`HTML`

```html
<div class="loading">Loading</div>
```

`CSS`
```css
.loading:after {
    overflow: hidden;
    display: inline-block;
    vertical-align: bottom;
    animation: ellipsis 2s infinite;
    content: "\2026";
    /* ascii code for the ellipsis character */
}

@keyframes ellipsis {
    from {
        width: 2px;
    }
    to {
        width: 15px;
    }
}
```
<b>浏览器支持</b>
<iframe src="https://caniuse.bitsofco.de/embed/index.html?feat=css-animation&amp;periods=future_2,future_1,current,past_1,past_2,past_3&amp;accessible-colours=false" frameborder="0" width="100%" height="465px"></iframe>
