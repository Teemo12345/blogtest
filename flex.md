## flex-direction -- 排列元素方向
> [row | row-reverse | column | column-reverse]
+ row 从左到右
+ row-reverse 从右到左
+ column 从上到下
+ column-reverse 从下到上

## flex-wrap  
### 元素包裹：默认情况下，项目都排在一条线（又称"轴线"）上，当排列不下时是否换行
> [nowrap | wrap | wrap-reverse]
+ nowrap 不换行
+ wrap 换行
+ wrap-reverse 换行，并且反转，第一行在下方

## flex-flow 此属性为flex-direction与flex-wrap的组合简写形式
> 默认值为 row nowrap

## justify-content 水平对齐方式
> [flex-start | center | flex-end | space-between | space-around]
+ flex-start 左对齐
+ center 居中对齐
+ space-between 两端对齐
+ space-around 平均分配，间距为两端间距的一倍

## align-items 垂直对齐方式
> [flex-start | center | flex-end | baseline | stretch]
+ flex-start 顶对齐(起始点对齐)
+ flex-end 底对齐
+ center 垂直居中
+ baseline 文字基线对齐
+ stretch 默认属性 拉长，撑满

## align-content 当垂直出现多行的时候，指定对齐方式，单行无效
> [flex-start | center | flex-end | space-between | space-around | stretch]
+ flext-start 顶部对齐
+ center 居中对齐
+ flex-end 底部对齐
+ space-between 顶底两端对齐
+ space-around 顶底平均分配对齐
+ stretch 默认值，填满容器，拉大。撑满容器

## [order | flex-grow | flex-shrink | flex-basis | flex | align-self]元素自身属性
+ order 排列顺序可指定，数值越小排列靠前，默认为0
+ flex-grow 放大比例属性；默认为0，存在空间也不放大。
+ flex-shrink 缩小比例属性；默认为1，如果空间不足将缩小。
+ flex-basis 属性定义了在分配多余空间之前，项目占据的主轴空间（main size）。浏览器根据这个属性，计算主轴是否有多余空间。它的默认值为auto，即项目的本来大小。
+ flex [flex-grow | flex-shrink | flex-basis] 三个属性的简写形式，默认值 flex: 0 1 auto;
+ align-self 可重置align-items属性，单独设置当前元素的垂直对齐方式