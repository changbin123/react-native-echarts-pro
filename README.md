
# react-native-echarts-pro
[![NPM Version](https://img.shields.io/npm/v/react-native-echarts-pro.svg?style=flat)](https://www.npmjs.com/package/react-native-echarts-pro)
[![NPM Version](https://img.shields.io/npm/dm/react-native-echarts-pro.svg?style=flat)](https://www.npmjs.com/package/react-native-echarts-pro)
[![license](https://img.shields.io/badge/license-MIT%20License-00AAAA.svg)](https://github.com/supervons/react-native-echarts-pro/blob/master/LICENSE)

English  [简体中文](/README_CN.md "中文介绍")
### A React-Native charts based on Apeach-Echarts.

## Getting started

`$ npm install react-native-echarts-pro --save`

It is super easy to `use echarts in react-native`. Have a look at our [Get Started Documentation](https://supervons.github.io/react-native-echarts-pro-docs/docs/intro) and onboard your app within minutes. Our detailed documentation is available as well.

## Documentation
[react-native-echarts-pro-docs](https://supervons.github.io/react-native-echarts-pro-docs/)

# Contributors

[@supervons](https://github.com/supervons)

[@ljh257110](https://github.com/ljh257110)

[@congshengwu](https://github.com/congshengwu)

[@RengeRenge](https://github.com/RengeRenge)
# 注意
为适配nkc-app项目的画图交互，修改了react-native-echarts-pro\src\components\Echarts\renderChart.js文件
使用myChart.getZr().on('click',()=>{})、myChart.getZr().on('mousemove',()=>{}),监听点击和移动，
获得点击像素点对应的柱状数，通过postmessage发送到RN，从而判断是否为主峰，添加Echarts的markLine画出核素峰指示线
