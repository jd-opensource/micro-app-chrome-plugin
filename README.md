# Micro-App-DevTools

<p align="center">
  <a href="https://jd-opensource.github.io/micro-app/">
    <img src="https://jd-opensource.github.io/micro-app/media/logo.png" alt="logo" width="100"/>
  </a>
</p>

# 📖简介
`Micro-App-DevTools`是基于京东零售推出的一款为`micro-app`框架而开发的`chrome`插件，旨在方便开发者对微前端进行数据查看以及调试,提升工作效率。

# 如何使用

在chrome中输入`chrome://extensions`打开扩展程序，打开[插件下载地址](https://github.com/jd-opensource/micro-app-chrome-plugin/releases)，选择最新Release包的`micro-app-chrome-plugin.zip`
文件下载，无需解压，将已下载的插件拖入。

在仅支持 `Manifest V3` 扩展的 Chrome 139+ 浏览器上，请使用 `Micro-App-DevTools V2+` 版本。

> 注：若仍需使用`Micro-App-DevTools V1+`版本，请在仍支持 `Manifest V2` 拓展的 Chrome 138 或更早版本浏览器的地址栏输入 `chrome://flags/#allow-legacy-mv2-extensions` 并启用允许加载旧版 `Manifest V2` 扩展选项。![扩展程序](https://zeromock.s3.cn-north-1.jdcloud-oss.com/micro-app/mv2.png)

![扩展程序](https://img12.360buyimg.com/imagetools/jfs/t1/119438/16/38287/53001/646b50e3F9012f2e8/3bba9844bbb1431b.png)

# 功能
打开控制台，选中`Micro app`

## 1、Environment环境

可查看`Micro app`的全局变量，目前显示的是最后一次加载的微应用信息，并支持点击具体条目跳转到官方文档说明。

![环境变量](https://zeromock.s3.cn-north-1.jdcloud-oss.com/micro-app/environment.png)

## 2、Communicate通讯
用于查看页面`Micro app`微应用结构、基本信息，以及模拟发送接收数据。
左侧展示的是页面微应用的层级结构，可选择对其进行操作。右侧上部显示当前应用的基本信息，包括名称、路由、iframe模式及版本号等信息。还可对其进行高亮标记，方便快速定位。
所有应用均支持模拟获取数据及发送数据，并可自动储存历史记录。

![通讯](https://zeromock.s3.cn-north-1.jdcloud-oss.com/micro-app/communicate.png)

## 3、路由信息
用于查看当前页面路由及MicroApp版本等信息

![路由](https://zeromock.s3.cn-north-1.jdcloud-oss.com/micro-app/communicate.png)

### 4、子应用开发环境模拟(仅插件 v1 版本支持)
点击按钮跳转至功能一中子应用开发环境模拟页面，此处模仿内嵌子应用，使用说明如下所示：

在子应用开发环境模拟页面中输入子页面`URL`等信息

> a、子页面URL：此处输入被基座应用嵌入的子应用链接

> b、父应用数据：此处输入JSON格式的父应用需要传给子应用的数据

> c、子应用嵌入代码：此处显示子应用嵌入的代码


以上即完成微前端的嵌入，效果如下：

![嵌入页面](https://zeromock.s3.cn-north-1.jdcloud-oss.com/micro-app/sub-app-simulation.png)

#### 快捷打开方式一
点击右上角图标出现目录,选择"打开子应用开发环境模拟"
![快捷方式](https://img12.360buyimg.com/imagetools/jfs/t1/99019/19/29391/10185/646b51dfF326dcc6c/04273f1a3daf9f9d.png)

#### 快捷打开方式二
点击鼠标右键，选择micro-app下，二级菜单点子应用开发环境模拟

![快捷方式](https://github.com/jd-opensource/micro-app-chrome-plugin/assets/14011130/91b40f7c-a826-4ffe-8c20-0b43a5c3bc6f)


## 常见问题
### 1、baseroute？
现象：插件系统的路由模块中，获取子应用链接功能与用户在嵌入微前端时是否使用到baseroute有很大的联系，如果用户配置了baseroute并且子应用路由确实使用了，则会获取正确的子应用链接，相反则可能会获取错误的子应用链接。

校正：若子应用与配置的baseroute无关联，建议删除配置顶baseroute。


## 🤝 参与共建

如果您对这个项目感兴趣，欢迎提[pull request](https://github.com/jd-opensource/micro-app-chrome-plugin/pulls)参与贡献，也欢迎 [Star](https://github.com/jd-opensource/micro-app-chrome-plugin) 支持一下 ^_^
欢迎小伙伴们加入`Micro-App-DevTools`微信群交流^ ^   

![image](https://github.com/user-attachments/assets/994ae21d-ad4f-47d5-8796-fe0bf892d89c)




