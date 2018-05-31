# 常见loading动画(纯CSS)

### 案例一：环形旋转

[效果页面](../assets/source/03_01-01Loading动画.html ':include :type=iframe width=100% height=220px')

[:point_right: 在codepen上编辑代码](https://codepen.io/shuangcs/pen/mLjGRE?editors=1100)

`HTML`

```html
<div class="item load-one">
  <div class="dount"></div>
</div>
```
`CSS`

```css
.item {
  width: 200px;
  height: 200px;
  background-color: #2980b9;
  display: table-cell;
  vertical-align: middle;
}
.dount {
  width: 50px;
  height: 50px;
  margin: 0 auto;
  border: 5px solid #80bfe9;
  border-left-color: #fff;
  border-radius: 50%; 
  animation: dount-anti 1.2s linear infinite;
}
@keyframes dount-anti {
  0% {transform: rotate(0deg)}
  100% {transform: rotate(360deg)}
}
```
### 案例二：上下波动

[效果页面](../assets/source/03_01-02Loading动画.html ':include :type=iframe width=100% height=220px')

[:point_right: 在codepen上编辑代码](https://codepen.io/shuangcs/pen/mLjGRE?editors=1100)

`HTML`

```html
<div class="item  load-three">
  <div class="jump">
    <div class="rect1"></div>
    <div class="rect2"></div>
    <div class="rect3"></div>
    <div class="rect4"></div>
    <div class="rect5"></div>
  </div>
</div>
```
`CSS`

```css
.item {
  width: 600px;
  height: 200px;
  background-color: #2980b9;
  display: table-cell;
  vertical-align: middle;
}
.load-three .jump {
    width: 80px;
    margin: 0 auto;
}
.load-three .jump > div {
  display:inline-block;
  width: 5px;
  height: 30px;
  background-color: #fff;
  animation: jump_anti 1.2s ease-in-out infinite;
}
.jump div.rect2 {
  -webkit-animation-delay: -1.1s;
  animation-delay: -1.1s;
}
 
.jump div.rect3 {
  -webkit-animation-delay: -1.0s;
  animation-delay: -1.0s;
}
 
.jump div.rect4 {
  -webkit-animation-delay: -0.9s;
  animation-delay: -0.9s;
}
 
.jump div.rect5 {
  -webkit-animation-delay: -0.8s;
  animation-delay: -0.8s;
}

@keyframes jump_anti {
  0%,40%,100% {
    transform: scaleY(0.4)
   }
  20% {
    transform: scaleY(1.0)
  }
}
```

### 案例三：环形圆球

[效果页面](../assets/source/03_01-03Loading动画.html ':include :type=iframe width=100% height=220px')

[:point_right: 在codepen上编辑代码](https://codepen.io/shuangcs/pen/wjxYKx)

`HTML`

```html
<div class="item">
  <div class="load-four circle">
    <div class="ball"></div>
    <div class="ball"></div>
    <div class="ball"></div>
    <div class="ball"></div>
    <div class="ball"></div>
    <div class="ball"></div>
    <div class="ball"></div>
    <div class="ball"></div>
  </div>
</div>
```
`CSS`

```css
.item {
  width: 1000px;
  height: 200px;
  background-color: #2980b9;
  display: table-cell;
  vertical-align: middle;
}
.load-four.circle {
  display:flex;
  justify-content: center;
  position: relative;
  width: 50px;
  height: 50px;
  margin: 0 auto;
}
.circle div.ball {
  width: 6px;
  height: 6px;
  border-radius:3px;
  background-color: #fff;
  position: absolute;
  animation: circle_anti 1.2s infinite alternate;
}
.circle div.ball:nth-child(1) {
  left: 24px;
  top: 2px;
  animation-delay: 0s;
}
.circle div.ball:nth-child(2) {
  top: 8px;
  left: 40px;
  animation-delay: 0.1s;
}
.circle div.ball:nth-child(3) {
  top: 24px;
  left:47px;
  animation-delay: 0.2s;
}
.circle div.ball:nth-child(4) {
  top: 40px;
  left: 40px;
  animation-delay: 0.3s;
}
.circle div.ball:nth-child(5) {
  top: 47px;
  left: 24px;
  animation-delay: 0.4s;
}
.circle div.ball:nth-child(6) {
  top: 40px;
  left: 8px;
  animation-delay: 0.5s;
}
.circle div.ball:nth-child(7) {
  top: 24px;
  left: 2px;
  animation-delay: 0.6s;
}
.circle div.ball:nth-child(8) {
  top: 8px;
  left: 8px;
  animation-delay: 0.7s;
}
@keyframes circle_anti {
  0%,40%,100%{
    transform: scale(1)
  }
  20% {
    transform: scale(2)
  }
}
```

### 案例四：进度条

[效果页面](../assets/source/03_01-04Loading动画.html ':include :type=iframe width=100% height=220px')

[:point_right: 在codepen上编辑代码](https://codepen.io/shuangcs/pen/ELpGLB)

`HTML`

```html
<div class="item">
        <div class="progress">
          <div class="loader-container"></div>
        </div>
      </div>
```
`CSS`

```css
.item {
  width: 1000px;
  height: 200px;
  background-color: #2980b9;
  display: table-cell;
  vertical-align: middle;
}
.load-four.circle {
  display:flex;
  justify-content: center;
  position: relative;
  width: 50px;
  height: 50px;
  margin: 0 auto;
}
.circle div.ball {
  width: 6px;
  height: 6px;
  border-radius:3px;
  background-color: #fff;
  position: absolute;
  animation: circle_anti 1.2s infinite alternate;
}
.circle div.ball:nth-child(1) {
  left: 24px;
  top: 2px;
  animation-delay: 0s;
}
.circle div.ball:nth-child(2) {
  top: 8px;
  left: 40px;
  animation-delay: 0.1s;
}
.circle div.ball:nth-child(3) {
  top: 24px;
  left:47px;
  animation-delay: 0.2s;
}
.circle div.ball:nth-child(4) {
  top: 40px;
  left: 40px;
  animation-delay: 0.3s;
}
.circle div.ball:nth-child(5) {
  top: 47px;
  left: 24px;
  animation-delay: 0.4s;
}
.circle div.ball:nth-child(6) {
  top: 40px;
  left: 8px;
  animation-delay: 0.5s;
}
.circle div.ball:nth-child(7) {
  top: 24px;
  left: 2px;
  animation-delay: 0.6s;
}
.circle div.ball:nth-child(8) {
  top: 8px;
  left: 8px;
  animation-delay: 0.7s;
}
@keyframes circle_anti {
  0%,40%,100%{
    transform: scale(1)
  }
  20% {
    transform: scale(2)
  }
}
```

[更多案例请参考:point_right: https://codepen.io/shuangcs/pen/mLKWdO](https://codepen.io/shuangcs/pen/mLKWdO)


