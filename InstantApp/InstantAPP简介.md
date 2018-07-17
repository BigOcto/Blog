# Instant App 简介

## 使用
通过URL分享APP部分功能，在用户无感知情况下，无安装使用app功能

## 限制
仅支持Android 6.0及以上系统，并且需要Google Service服务

## 开发
- Android studio 3.0 开发
- 可以重用之前app的代码,修改配置项，将工程设置为不同的feature modules，增加APP Links
- 上传至Google play

## 特点
- 模块化APP，将独立的APP分成多个Modules，也就是说， 将原有的一个APK模式，划分为多个 Instant APKS

## Android Studio 3.0 开发简介
- 生成URL-Mapping
- 可对通过URL打开的链接进行拦截，处理相关逻辑
- 创建App-Module,Base-Module,Base module build.gradle 中新加

  ```gradle
  dependencies{
    application project(":app-module")
  }
  Android{
    baseFeature true
  }
  ```
- 创建 Instant-module

- 创建 feature-module
