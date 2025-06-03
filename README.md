# Wechat-miniprogram

## 1.整体框架
- 后端（后端接口）
  - python：**flask**、django框架、fastapi框架
  - go：gin框架、beego框架
  - java：ssh框架、ssm框架、SpringBoot框架

- 前端（大前端）
  - web页面（浏览器中的页面）：html, css, js
  - 安卓/iso 的 app ：java, object C
  - **微信小程序：wxml, wxss, js**
  - 桌面端：qt平台（python, C++）

  - uni-app: 使用 html, css, js 以及 vue 的语法，在uni-app平台开发，打包到安卓，ios，微信小程序，web端
 
## 2.微信开发者工具介绍
### 2.1 项目主配置文件（在项目根目录下）
  - app.js（小程序入口文件，小程序启动时执行）
  - app.json（小程序的全局配置）
  - app.wxss（小程序的全局样式）
    
### 2.2 页面文件
- **pages 文件夹**（其中包含数个文件夹，每个文件夹代表一个页面，其下有4个文件）
  - index
    - index.js（页面逻辑，js代码控制）
    - index.wxml（页面结构，布局，约等同于html）
    - index.json（页面配置，如当前页面顶部颜色、标题等）
    - index.wxss（页面样式）
  - login
  ...
- **components 文件夹**（页面中会用到的组件，其中包含数个文件夹，每个文件夹代表一个组件，其下有4个文件）
- **eslintrc.js**：语法检查
- **project.config.json** & **project.private.config.json**：项目基础配置（存放位置、是否开启https等）
- **sitemap.json**：搜索优化（用户可以通过什么关键词搜到该app）

![image](https://github.com/user-attachments/assets/20c5f84a-f2ce-4266-bd18-095797f668ee)

### 2.3 配置文件
#### 2.3.1 全局配置 app.json
参考地址：https://developers.weixin.qq.com/miniprogram/dev/reference/configuration/app.html  
  - entryPagePath（小程序默认启动首页）
  - pages（小程序总共有多少个页面）
  - **window** （全局的默认窗口表现，顶部颜色，是否有下拉）
    
#### 2.3.2 页面配置 xx.json
参考地址：https://developers.weixin.qq.com/miniprogram/dev/reference/configuration/page.html  
  - navigationBarBackgroundColor （导航栏背景颜色，如 #000000）
  - navigationBarTextStyle （导航栏标题、状态栏颜色，仅支持 black / white ）
  - navigationBarTitleText （导航栏标题文字内容）
 
#### 2.3.3 工程配置 project.config.json, project.private.config.json
参考地址：https://developers.weixin.qq.com/miniprogram/dev/devtools/projectconfig.html  

#### 2.3.4 搜索相关配置 sitemap.json
参考地址：https://developers.weixin.qq.com/miniprogram/dev/reference/configuration/sitemap.html  
默认配置：以后用户搜索小程序，任意页面有关键词都会被搜索到

### 2.4 小程序常用组件 components   
参考地址：https://developers.weixin.qq.com/miniprogram/dev/component/  
对标 html 中的标签（a, div, span, img...）
  - text 对标 span （不换行，放文字）
  - view 对标 div （换行）
  - image 对标 img
... 


