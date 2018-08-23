### 目录解构
```
-- 📂assets
  -- 📂font // 字体文件存放
  -- 📂iconfont // 字体图标存放
  -- 📂scss
    -- 📂variables // 变量
      -- 📃variables.scss //公共变量
      -- 📃table.scss // 个体变量，根据模块命名
      -- ......
    -- 📂mixins // 混合宏
      -- 📃mixins.scss // 公共宏
      -- 📃table.scss // 文件个体宏，根据模块命名
      -- ......
    -- 📂element-replace // 替换element UI的样式
      -- 📃element.scss // 替换样式
    -- 📂modle // 根据模块名称命名
      -- 📃modle.scss // 根据模块名称命名
      -- ......
    -- 📃common.scss // 公共样式
    -- 📃font.scss // 字体
    
```

### 变量定义
```
-- 📃variables.scss
      // colors
      $white:       #fff !default;
      $black:       #000 !default;
      $body-bg:     $white !default;
      $body-color:  $black !default;
      ......
------------------------------------------------------------
-- table.scss
    $table-bg: $white;
    ......
```

### 混合宏定义
      // colors
