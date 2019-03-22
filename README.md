# css

## rules
开发中样式表的规范说明

## 字体
```
字体大小样式可选以下样式-------------------------
$font-size: (12, 14, 16, 18, 20, 22, 24, 26,
28, 30, 32, 34, 36, 38, 40, 42,
44, 46, 48, 50, 52, 54, 56, 58, 60, 62,
64, 66, 68, 70, 72, 74, 76, 78);
@each $size in $font-size {
  .font-size-#{$size} {
    font-size: #{$size}px;
  }
}
举例：
font-size-12
font-size-14
...
font-size-78

字体粗细--------------------------------------------------------
font-weight-bold 
font-weight-normal

字体颜色---------------------------------------------------------
font-color-normal      // 默认字体颜色#54585A
font-color-title       // 标题字体颜色#2A2C2D
font-color-description // 描述字体颜色#7E8487

字体对齐方式-------------------------------------------------------
text-align-left        // 左对齐
text-align-right       // 右对齐
text-align-center      // 居中对齐

字体截取-----------------------------------------------------------
$text-overflow-ellipsis-size: (2, 3, 4, 5, 6, 7, 8, 9, 10)
text-overflow-ellipsis   // 单行截取
text-overflow-ellipsis-2 // 多行截取
```
## 间距
```
$space: (6, 8, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 
32, 34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56, 58, 60);
举例：
margin-left-6
margin-right-6
margin-top-6
margin-bottom-6
padding-left-6
padding-right-6
padding-top-6
padding-bottom-6
```

## 布局
```
宽高
width-100
height-100

滚动条
overflow-hidden
overflow-auto



```

