### 目录解构
```
-- assets
  -- font // 字体文件存放
  -- iconfont // 字体图标存放
  -- styles
    -- variables.scss // 变量
    -- mixins.scss // 混合宏
    -- elereset // 替换element UI的样式
    -- font.scss // 字体
    -- reset.scss // 重置样式
    -- common.scss // 公共样式
    
```

### 变量定义

> 公共变量定义表
```
-- variables.scss
      // Color system
      $white: #fff !default;
      $gray-100: #f8f9fa !default;
      $gray-200: #e9ecef !default;
      $gray-300: #dee2e6 !default;
      $gray-400: #ced4da !default;
      $gray-500: #adb5bd !default;
      $gray-600: #6c757d !default;
      $gray-700: #54585A !default;
      $gray-800: #343a40 !default;
      $gray-900: #212529 !default;
      $black: #000 !default;
      $blue: #007bff !default;
      $indigo: #6610f2 !default;
      $purple: #6f42c1 !default;
      $pink: #e83e8c !default;
      $red: #dc3545 !default;
      $orange: #fd7e14 !default;
      $yellow: #ffc107 !default;
      $green: #28a745 !default;
      $teal: #20c997 !default;
      $cyan: #17a2b8 !default;
      ......
   ---------------------------------------------------------
      // body
      $body-bg: $white !default;
      $body-color: $gray-700 !default;
      ......
   ---------------------------------------------------------
      // font
      $font-size-base: 1rem !default;
      ......
```

### 混合宏

> 公用样式
```
-- mixins.scss
  // 单行文字截取...
  @mixin text-overflow {
    text-overflow: ellipsis;
    overflow: hidden;
    white-space: nowrap;
  }
  // 多行文字截取...
  @mixin text-overflow-clamp($clamp: 2) {
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -o-text-overflow: ellipsis;
    text-overflow: ellipsis;
    -webkit-line-clamp: $clamp;
    overflow:hidden;
  }
  ......
```

### 重置

> 重置浏览器内置样式
```
-- reset.scss
  * {
    margin: 0;
    padding: 0;
    word-break: break-all;
    box-sizing: border-box;
  }

  ul, ol, li {
    list-style: none;
    margin: 0;
    padding: 0;
  }

  img {
    vertical-align: middle;
    border: 0;
  }
  ......
```

### 字体

> 自定义字体样式
```
@font-face {
  font-family: 'NotoSansCJKsc';
  src: url("../font/NotoSansCJKsc-Light.ttf") format("truetype"),
  url("../font/NotoSansCJKsc-Light.woff");
  font-weight: normal;
  font-style: normal;
}

body {
  font-family: "BlueSkyStandardLight",
  "NotoSansCJKsc",
  "PingFang SC", "PingHei",
  "Microsoft YaHei",
  sans-serif;
}
```

### 全局样式
```
-- common.scss
  @import "variables";
  @import "font";
  @import "reset";
  @import "elereset";
  @import "iconfont/iconfont";

  body {
    font-size: $font-size-base;
    background: $body-bg;
    color: $body-color;
  }
  ......
```
