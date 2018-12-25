# bc-css-layout
bc-css-layout H5，小程序页面布局样式等
感觉不应用样式布局，都不会写页面了，MMP~,css布局样式主要参考[ionic框架样式](https://ionicframework.com/docs/api/components/grid/Grid)

# 使用
均已以`bc-` 开头;

# 简介
## css rest
小程序没有所谓的html标签概念，所以不需要！
H5端可以
略~

## 常用的css 集合




## flex 布局
```html
 <View className="row justify-content-around">
	<View className="col align-self-start">
	  <Text>1 of 4</Text>
	  <View className="row justify-content-between">
		<View className="col align-self-start">
		  <Text>1 of 4</Text>
		</View>
		<View className="col align-self-end">
		  <Text>3 of 4</Text>
		</View>
	  </View>
	</View>
	<View className="col align-self-center">
	  <Text>2 of 4</Text>
	</View>
	<View className="col align-self-end">
	  <Text>3 of 4</Text>
	</View>
	<View className="col">
	  <Text>
		4 of 4 <Text>#</Text>
		<Text>#</Text>#
	  </Text>
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
小程序不支持 子选择符 `>`，支持id、class这类选择器，足以~
不要使用属性选择符，对于Taro这会不支持
推荐`class`。


# 参考

[小程序组件化解决方案](http://www.wetouch.net/touchwx_doc/transform/transform/transform)。


