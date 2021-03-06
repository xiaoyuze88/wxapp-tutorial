# 大纲

## 序章

本课程适合有一定前端基础的同学，熟悉HTML5, CSS3, JavaScript (ES6/ES7)，对小程序有兴趣或有实际开发需求，希望能够通过本课程熟悉小程序并能够快速进入生产环境产出。

本课程主要从中大型小程序开发项目实践中总结实战经验，一步一步引导大家从熟悉什么是小程序，到如何架构及设计一个有一定规模的小程序项目。

本课程并不会详细介绍所有小程序提供的组件及API，具体用法都可以在官方文档中查阅，一些常用或有坑的Api会在课程中穿插介绍。

本课程项目中使用的服务端使用 NodeJS ，仅用于课程教学使用，并不会对NodeJS做过多介绍，生产环境中的 Backend 需要根据实际情况选择。

## 第1章 简介

介绍什么是小程序，包括小程序的特点、特性及简介本课程包含的内容

## 第2章 搭建小程序客户端本地开发环境

包括如何申请个人开发账号；

小程序开发工具的下载、安装、主要功能简介；

小程序项目依赖的本地环境的安装，项目脚手架安装、部署，基于NodeJS的服务端的安装与部署。

最终能够在本地工具中跑起项目，并能够在手机中预览。

## 第3章 小程序开发基础入门介绍

从脚手架项目出发，介绍小程序的基本目录结构、基本配置，WXML、WXSS文件以及与HTML、CSS的异同，RPX单位，一些最常用的基础视图组件，Page的生命周期，单向数据流等小程序开发基础知识。

最后简要介绍小程序的一些底层原理，让大家对小程序是什么，项目是如何跑起来的有一个基本概念。

## 第4章 开始开发第一个小程序

开始开发第一个小程序，从页面详细配置，到整体布局、tab的设置及使用、基础视图的拼装、scroll-view的使用等等，从实践中体会小程序开发。

## 第5章 准备就绪，开始进入生产环境

原生的小程序，无论是从小程序Api的设计上还是从设计模式上都不利于大型项目的开发与维护。准备进入生产环境，引入Babel与Less，并引入设计模式。

介绍脚手架项目中使用的构建流，以及我们对项目包大小优化做出的研究。引入ES6与Less，增加项目的可维护性，引入设计模式，介绍页面的继承、基类的抽象以及“组件”及其实现原理。

最后将上一个项目重构为引入构建流及设计模式之后的模式，体会与介绍生产环境中引入这些元素的优势。

## 第6章 进阶，开始开发更复杂的模块

从我们实际项目中挑选几个典型的场景，带领大家学习开发，包括带有选择器的无限滚动列表，两种带有自定义Tab的页面，表单页面的使用等。

## 第7章 登录态

除去一些纯工具类应用，绝大部分小程序都需要用到登录态，来识别用户身份。

小程序中的登录态分为两个概念，一个是微信自己的用户的登录态、一种是开发者自行维护的登录态。

传统意义上一般讨论小程序的登录态都是微信自己的登录态，由微信自行维护，由开发者保持登录态具体信息。

另一种是业务本身有自己的登录态体系，借助微信的openId或unionId来维系其微信用户与业务登录态的关系，业务自行维护登录态（最典型的就是腾讯视频小程序，同时支持微信登陆及QQ登陆，分别对应着这两种登陆态）。

本章将分别介绍这两种登录态的流程、原理、实现及一些细节，并介绍openId与unionId的概念。

最后介绍我们自己在实现小程序与腾讯云登录态打通中做的工作，包括自行实现Cookie，对request api的封装，以及unionId与腾讯云帐号绑定关系的实现等等。

## 第8 结合腾讯云小程序解决方案使用

对于个人开发者，后端服务的稳定性、运维、https证书等将会是开发小程序中的最大障碍。

腾讯云小程序解决方案专门针对个人开发者提供了一套一键部署后端环境的服务，官方小程序开发工具中也已经集成了腾讯云小程序解决方案中的一些配套能力。

本章将对如何使用该解决方案来快速部署可运用于生成环境的后端服务做简单介绍。

## 第9 一些开发过程中的细节、经验分享与注意事项

- 小程序中的图表(Canvas)
- 小程序中的微信支付
- 一些性能、体验优化的技巧
- 基础库兼容性的处理
- 请求用户授权及用户拒绝后的容错处理
- 上线审核的注意事项
- 发布流程与版本管理的经验分享
- 运营、数据分析与数据上报

## 总结

总结个人开发小程序大半年对小程序开发的体验与心得，并介绍一些最新发布尚有严重版本兼容性问题不建议大规模使用的组件及未来展望。
