
# react-native-echarts-pro
[![NPM Version](https://img.shields.io/npm/v/react-native-echarts-pro.svg?style=flat)](https://www.npmjs.com/package/react-native-echarts-pro)
[![NPM Version](https://img.shields.io/npm/dm/react-native-echarts-pro.svg?style=flat)](https://www.npmjs.com/package/react-native-echarts-pro)
[![license](https://img.shields.io/badge/license-MIT%20License-00AAAA.svg)](https://github.com/supervons/react-native-echarts-pro/blob/master/LICENSE)

[English](/README.md "english readme")  简体中文
###  基于 Apeach-Echarts 的 React-Native 图表库.

## 开始

`$ npm install react-native-echarts-pro-nkc-app --save`

在你的RN项目中接入 `echarts` 非常简单，查看 [开始文档](https://supervons.github.io/react-native-echarts-pro-docs/zh-cn/docs/intro)。

## 详细文档
[react-native-echarts-pro-docs](https://supervons.github.io/react-native-echarts-pro-docs/zh-cn/)

## 贡献者

[@supervons](https://github.com/supervons)

[@ljh257110](https://github.com/ljh257110)

[@congshengwu](https://github.com/congshengwu)

[@RengeRenge](https://github.com/RengeRenge)
## 注意
修改一：
\src\components\Echarts\renderChart.js文件进行了针对性修改
修改了click事件点击获取相应像素点的柱状图列数，发送到RN；添加的mousemove一样
修改二：
在renderChart.js中的addEventListener监听message中添加如下代码，支持formatter的字符串转化函数方式
option.yAxis.axisLabel.formatter = eval("(" + option.yAxis.axisLabel.formatter + ")");
