# v5-css-layout

v5-css-layout H5、小程序页面布局样式等
css 布局样式主要参考[ionic 框架样式](https://ionicframework.com/docs/api/components/grid/Grid)

~感觉不应用样式布局，都不会写页面了，MMP~

`icon.scss` 以`v5-` 开头

# 使用

目前个人主要使用 [Taro](https://github.com/NervJS/taro)，进行开发，打算使用 Taro 结合改样式开发一些页面，待计划~

略~

# 简介

## css rest

小程序没有所谓的 html 标签概念，所以不需要！
H5 端可以
略~

## 常用的 css 集合

## flex 布局

```html
<View className="row justify-content-around">
    <View className="col align-self-start">
        <Text>1 of 4</Text>
        <View className="row justify-content-between">
            <View className="col align-self-start"> <Text>1 of 4</Text> </View>
            <View className="col align-self-end"> <Text>3 of 4</Text> </View>
        </View>
    </View>
    <View className="col align-self-center"> <Text>2 of 4</Text> </View>
    <View className="col align-self-end"> <Text>3 of 4</Text> </View>
    <View className="col">
        <Text> 4 of 4 <Text>#</Text> <Text>#</Text># </Text>
    </View>
</View>
```

也可在外层包裹 `className="grid"`

## 图标

# 演示示例

```
.grid-basic-page ion-col div {
    background-color: #f0f5ff;
    border: 1px solid #e6e9ee;
    border-radius: 2px;
    padding: 5px;
    text-align: center;
}
```

```
<ui-row border-top border-bottom height="40" space-bottom="20">
        <ui-col border-right align="center"  hover-stop-propagation vertical-align="middle">25%</ui-col>
        <ui-col border-right align="center"  vertical-align="middle">25%</ui-col>
        <ui-col border-right align="center" vertical-align="middle">25%</ui-col>
        <ui-col align="center" vertical-align="middle">25%</ui-col>
</ui-row>
```

# 问题？

小程序不支持 子选择符 `>`，支持 id、class 这类选择器，足以~
不要使用属性选择符，对于 Taro 这会不支持
推荐`class`。

# TODO

-   使用 `Taro` 完成该库的相关页面实现
-   常用组件制作~
-   添加封装相应功能库，如统一请求 request 拦截等

# 参考

[小程序组件化解决方案](http://www.wetouch.net/touchwx_doc/transform/transform/transform)。
