# JLU iEdu Android

吉林大学 iEdu 教务门户 Android 客户端。应用使用 Android WebView 加载：

https://iedu.jlu.edu.cn/jwapp/sys/emaphome/portal/index.do

## 功能

- 应用内打开 iEdu 教务门户
- 支持 JavaScript、DOM Storage、Cookie 登录态
- 顶部加载进度条
- 页面加载失败提示与点击重试
- Android 返回键回退网页历史
- 非 HTTP/HTTPS 链接交给系统应用处理

## 隐私与安全

本项目只是网页容器，不内置账号、密码或学校接口密钥。登录信息由学校网站和 Android WebView/Cookie 机制处理。不要把个人账号密码提交到仓库、Issue 或截图中。

## 构建

用 Android Studio 打开项目，或在命令行运行：

```bash
./gradlew assembleDebug
```

如果本地没有 Gradle Wrapper，也可以在安装 Gradle 后运行：

```bash
gradle assembleDebug
```

## GitHub Actions

仓库包含一个 Android 构建工作流。推送到 `main` 后会自动构建 debug APK，并上传为 Actions artifact。

## 说明

该项目不是吉林大学官方应用，仅为指定网站的移动端封装示例。
