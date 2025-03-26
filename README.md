# Custom Slider
Three Panel Custom Slider Section For Shopify

Section > create custom-slider.liquid as a section file  
Owl Carousel 配置项文档  
基本配置项  
items: Number  
默认值: 3  
轮播中显示的项目数量。  
loop: Boolean  
默认值: false  
是否循环播放。  
center: Boolean  
默认值: false  
是否将当前活动项目居中显示。  
rewind: Boolean  
默认值: false  
在到达末尾时是否重回开头。  
mouseDrag: Boolean  
默认值: true  
是否允许鼠标拖动。  
touchDrag: Boolean  
默认值: true  
是否允许触摸拖动。  
pullDrag: Boolean  
默认值: true  
是否允许拉动拖动。  
freeDrag: Boolean  
默认值: false  
是否允许自由拖动。  
margin: Number  
默认值: 0  
项目之间的间距。  
stagePadding: Number  
默认值: 0  
轮播的外边距。    
merge: Boolean  
默认值: false  
是否启用项目合并功能。  
autoWidth: Boolean  
默认值: false  
是否自动计算项目宽度。  
startPosition: Number  
默认值: 0  
设置初始显示的项目索引。  
rtl: Boolean  
默认值: false  
是否启用右到左的布局。  
smartSpeed: Number  
默认值: 250  
动画速度，单位为毫秒。  
fluidSpeed: Boolean  
默认值: false  
是否启用流动动画。  
dragEndSpeed: Boolean  
默认值: false  
拖动结束时的动画速度。   
响应式设置  
responsive: Object  
定义在不同屏幕宽度下的配置项。  
示例：  
javascript
```
responsive: {
    0: {
        items: 1
    },
    600: {
        items: 2
    },
    1000: {
        items: 3
    }
}
```

responsiveRefreshRate: Number 
默认值: 200  
响应式刷新率，单位为毫秒。  
responsiveBaseElement: Element  
默认值: window  
用于计算响应式设置的基准元素。  
额外功能  
fallbackEasing: String  
默认值: "swing"  
动画的缓动效果。  
info: Boolean  
默认值: false  
是否显示信息。  
nestedItemSelector: String  
默认值: false  
嵌套项目选择器。  
itemElement: String  
默认值: "div"  
项目的 HTML 元素类型。  
stageElement: String  
默认值: "div"  
轮播的舞台元素类型。  
refreshClass: String  
默认值: "owl-refresh"  
刷新时应用的类名。  
loadedClass: String  
默认值: "owl-loaded"  
加载完成时应用的类名。  
loadingClass: String  
默认值: "owl-loading"  
加载中时应用的类名。  
rtlClass: String  
默认值: "owl-rtl"  
RTL 模式时应用的类名。  
responsiveClass: String  
默认值: "owl-responsive"  
响应式模式时应用的类名。  
dragClass: String  
默认值: "owl-drag"  
拖动时应用的类名。
itemClass: String
默认值: "owl-item"
项目的类名。
stageClass: String
默认值: "owl-stage"
舞台的类名。
stageOuterClass: String
默认值: "owl-stage-outer"
外部舞台的类名。
grabClass: String
默认值: "owl-grab"
鼠标悬停时应用的类名。
使用示例
javascript

复制
$('.owl-carousel').owlCarousel({
    items: 1,
    loop: true,
    margin: 10,
    responsive: {
        0: {
            items: 1
        },
        600: {
            items: 2
        },
        1000: {
            items: 3
        }
    }
});
这个文档概述了 Owl Carousel 的主要配置项及其用途，便于用户快速理解和使用。

# Owl Carousel 配置项文档

## 基本配置项

- **items**: `Number`
  - 默认值: `3`
  - 轮播中显示的项目数量。

- **loop**: `Boolean`
  - 默认值: `false`
  - 是否循环播放。

- **center**: `Boolean`
  - 默认值: `false`
  - 是否将当前活动项目居中显示。

- **rewind**: `Boolean`
  - 默认值: `false`
  - 在到达末尾时是否重回开头。

- **mouseDrag**: `Boolean`
  - 默认值: `true`
  - 是否允许鼠标拖动。

- **touchDrag**: `Boolean`
  - 默认值: `true`
  - 是否允许触摸拖动。

- **pullDrag**: `Boolean`
  - 默认值: `true`
  - 是否允许拉动拖动。

- **freeDrag**: `Boolean`
  - 默认值: `false`
  - 是否允许自由拖动。

- **margin**: `Number`
  - 默认值: `0`
  - 项目之间的间距。

- **stagePadding**: `Number`
  - 默认值: `0`
  - 轮播的外边距。

- **merge**: `Boolean`
  - 默认值: `false`
  - 是否启用项目合并功能。

- **autoWidth**: `Boolean`
  - 默认值: `false`
  - 是否自动计算项目宽度。

- **startPosition**: `Number`
  - 默认值: `0`
  - 设置初始显示的项目索引。

- **rtl**: `Boolean`
  - 默认值: `false`
  - 是否启用右到左的布局。

- **smartSpeed**: `Number`
  - 默认值: `250`
  - 动画速度，单位为毫秒。

- **fluidSpeed**: `Boolean`
  - 默认值: `false`
  - 是否启用流动动画。

- **dragEndSpeed**: `Boolean`
  - 默认值: `false`
  - 拖动结束时的动画速度。

## 响应式设置

- **responsive**: `Object`
  - 定义在不同屏幕宽度下的配置项。
  - 示例：
    ```javascript
    responsive: {
        0: {
            items: 1
        },
        600: {
            items: 2
        },
        1000: {
            items: 3
        }
    }
    ```

- **responsiveRefreshRate**: `Number`
  - 默认值: `200`
  - 响应式刷新率，单位为毫秒。

- **responsiveBaseElement**: `Element`
  - 默认值: `window`
  - 用于计算响应式设置的基准元素。

## 额外功能

- **fallbackEasing**: `String`
  - 默认值: `"swing"`
  - 动画的缓动效果。

- **info**: `Boolean`
  - 默认值: `false`
  - 是否显示信息。

- **nestedItemSelector**: `String`
  - 默认值: `false`
  - 嵌套项目选择器。

- **itemElement**: `String`
  - 默认值: `"div"`
  - 项目的 HTML 元素类型。

- **stageElement**: `String`
  - 默认值: `"div"`
  - 轮播的舞台元素类型。

- **refreshClass**: `String`
  - 默认值: `"owl-refresh"`
  - 刷新时应用的类名。

- **loadedClass**: `String`
  - 默认值: `"owl-loaded"`
  - 加载完成时应用的类名。

- **loadingClass**: `String`
  - 默认值: `"owl-loading"`
  - 加载中时应用的类名。

- **rtlClass**: `String`
  - 默认值: `"owl-rtl"`
  - RTL 模式时应用的类名。

- **responsiveClass**: `String`
  - 默认值: `"owl-responsive"`
  - 响应式模式时应用的类名。

- **dragClass**: `String`
  - 默认值: `"owl-drag"`
  - 拖动时应用的类名。

- **itemClass**: `String`
  - 默认值: `"owl-item"`
  - 项目的类名。

- **stageClass**: `String`
  - 默认值: `"owl-stage"`
  - 舞台的类名。

- **stageOuterClass**: `String`
  - 默认值: `"owl-stage-outer"`
  - 外部舞台的类名。

- **grabClass**: `String`
  - 默认值: `"owl-grab"`
  - 鼠标悬停时应用的类名。

## 使用示例

```javascript
$('.owl-carousel').owlCarousel({
    items: 1,
    loop: true,
    margin: 10,
    responsive: {
        0: {
            items: 1
        },
        600: {
            items: 2
        },
        1000: {
            items: 3
        }
    }
});
