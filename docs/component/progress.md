#### progress
进度条。

**属性说明**

|属性名			|类型		|默认值		|说明													|平台差异说明				|
|:-				|:-			|:-			|:-														|:-						|
|percent		|Float		|无			|百分比0~100											|						|
|show-info		|Boolean	|false		|在进度条右侧显示百分比									|						|
|border-radius|number/string|0|圆角大小|微信基础库2.3.1+、QQ小程序|
|font-size|number/string|16|右侧百分比字体大小|微信基础库2.3.1+、QQ小程序|
|stroke-width	|Number		|6			|进度条线的宽度，单位px									|						|
|activeColor	|Color		|#09BB07（百度为#E6E6E6）	|已选择的进度条的颜色									|						|
|backgroundColor|Color		|#EBEBEB	|未选择的进度条的颜色									|						|
|active			|Boolean	|false		|进度条从左往右的动画									|						|
|active-mode	|String		|backwards	|backwards: 动画从头播；forwards：动画从上次结束点接着播|App、H5、微信小程序、QQ小程序	|
|duration|number|30|进度增加1%所需毫秒数|微信基础库2.8.2+|
|@activeend		|EventHandle|			|动画完成事件											|微信小程序				|

**示例** [查看演示](https://uniapp.dcloud.io/h5/pages/component/progress/progress)
```html
<template>
	<view>
		<view class="uni-padding-wrap uni-common-mt">
			<view class="progress-box">
				<progress percent="20" show-info stroke-width="3" />
			</view>
			<view class="progress-box">
				<progress percent="40" active stroke-width="3" />
			</view>
			<view class="progress-box">
				<progress percent="60" active stroke-width="3" backgroundColor="#999"/>
			</view>
			<view class="progress-box">
				<progress percent="80" activeColor="red" active stroke-width="8" />
			</view>
		</view>
	</view>
</template>
```

![](https://img-cdn-qiniu.dcloud.net.cn/uniapp/doc/img/propress.png)
