1. ` @extend` 语法
```scss
.circle-2 {
    @extend .circle-1; // 继承 .circle-1 类的所有样式
    width: 82px;       // 设置元素的宽度为82像素
    height: 82px;      // 设置元素的高度为82像素
    top: -6px;         // 设置元素的顶部偏移为-6像素
    left: -6px;        // 设置元素的左侧偏移为-6像素
    border-color: $brown transparent $brown $brown; // 设置元素的边框颜色，使用Sass变量 $brown 和透明色
}
```


2. 

```scss
.box {
    box-sizing: border-box; // 设置盒模型为border-box，包含内边距和边框
    width: 120px;           // 设置元素的宽度为120像素
    height: 99px;           // 设置元素的高度为99像素
    background: #F5E8DF;    // 设置元素的背景颜色为#F5E8DF
    text-align: center;     // 设置文本居中对齐
    padding-top: 28px;      // 设置顶部内边距为28像素
    transition: all .4s ease-in-out; // 设置所有属性的过渡效果，持续时间为0.4秒，缓动函数为ease-in-out

    &:hover {
        background: #E1CFC2; // 当鼠标悬停时，背景颜色变为#E1CFC2
        cursor: pointer;     // 当鼠标悬停时，光标变为指针形状
    }

    // 偶数个元素
    &:nth-child(2) {
        margin: 1px 0; // 针对第2个子元素，设置上下外边距为1像素
    }
}

```