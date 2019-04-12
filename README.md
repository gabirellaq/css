# css

## rules
开发中样式表的规范说明

## 字体
```
字体大小
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

字体粗细
font-weight-bold 
font-weight-normal

字体颜色
font-color-normal      // 默认字体颜色#54585A
font-color-title       // 标题字体颜色#2A2C2D
font-color-description // 描述字体颜色#7E8487

字体对齐方式
text-align-left        // 左对齐
text-align-right       // 右对齐
text-align-center      // 居中对齐

字体截取
$text-overflow-ellipsis-size: (2, 3, 4, 5, 6, 7, 8, 9, 10)
text-overflow-ellipsis   // 单行截取...
text-overflow-ellipsis-2 // 多行截取...
```

## color
```
color-black         // color #000;
color-black-2A      // color #2A2C2D;
color-grey-54       // color #54585A;
color-grey-7E       // color #7E8487;
color-grey-DC       // color #dcdcdc;
color-white         // color #fff;
color-white-8       // color #f8f8f8;
color-nio           // color #00BCBC;
color-danger        // color #FF231E;
color-success       // color #28a745;
color-warning       // color #ffc107;
color-rose-red      // color #e83e8c;
```

## 背景
```
background-color-white     // 背景白色
background-color-white-8   // 背景 #f8f8f8
```

## 间距
```
$space: (6, 8, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 
32, 34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56, 58, 60);
举例：
margin-6
margin-left-6
margin-right-6
margin-top-6
margin-bottom-6
padding-6
padding-left-6
padding-right-6
padding-top-6
padding-bottom-6
```

## 边框
```
border-left     // 1px solid #dcdcdc
border-right
border-top
border-bottom
```

## 圆角
```
$border-radius: (4, 6, 8, 10, 12, 14, 16, 18, 20);
border-radius-4        // border-raius: 4px;
...
border-radius-20
border-radius-left-4   // border-radius: 0 0 0 4px;
border-radius-right-4
border-radius-top-4
border-radius-bottom-4
...
```

## 布局
```
宽高
width-100
height-100

滚动条
overflow-hidden
overflow-auto

布局
display-flex                   // flex布局 默认横向排列，双轴靠左
display-flex-column            // flex布局 竖向排列，双轴靠左
align-items-center             // 元素在侧轴居中
align-items-flex-end           // 元素向侧轴终点对齐
justify-content-center         // 主轴 居中排列
justify-content-space-around   // 主轴 均匀排列每个元素 每个元素周围分配相同的空间
justify-content-space-between  // 主轴 均匀排列每个元素 首个元素放置于起点，末尾元素放置于终点
justify-content-flex-end       // 主轴 从行尾位置开始排列
flex-wrap                      // 换行
flex-wrap-reverse              // 反向换行

$flex: (1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12);
flex-1                         // 弹性元素的伸缩比
flex-2
flex-3
...
flex-12

```

