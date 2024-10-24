+++
title = 'typora 破解'
date = 2024-09-23T16:59:07+08:00
draft = false
+++

typora 破解版

> 之前发布的算法破解已经失效。提示版本过低。这次更新一下最新版本如何破解教程

# Typora v1.9.5 激活

安装Typora([https://typoraio.cn/](https://lb5.net/go/aHR0cHM6Ly90eXBvcmFpby5jbi8)) 打开官网 下载并安装最新版即可，这里不再提供安装包

# 修改文件

打开 **Typora路径**下这个js文件夹

**♾️ html 代码:**

```html
typora\resources\page-dist\static\js
```

文件夹中找到两个**LicenseIndex**开头的两个文件，然后用**VSCODE**打开，然后右键点击格式化文档，方便查看。

然后把这两个**LicenseIndex**文件中的代码替换掉

**♾️ js 代码:**

```js
e.hasActivated="true"== e.hasActivated
```

替换成下面代码

**♾️ js 代码:**

```js
e.hasActivated="true"=="true"
```

重点 **两个文件都要这样替换**后保存一下

# 关闭软件已激活弹窗

找到以下路径,同样方法打开**license.html**文件

**♾️ text 代码:**

```text
resources\page-dist\license.html
```

将替换成下面代码

**♾️ html 代码:**

```html
</body>
<script>
window.οnlοad=function(){setTimeout(()=>{window.close();},5);}
</script>
</html>
```

保存一下

# 去除软件左下角未激活提示文字

依旧是打开下面路径的**Panel.json**文件
**resources\locales\zh-Hans.lproj\Panel.json**

将**"UNREGISTERED":"未激活"**替换成**"UNREGISTERED":" "** 保存一下

# 截图

![screenshots.gif](https://lb5-1318274915.cos.ap-shanghai.myqcloud.com//usr/uploads/2024/09/1699615544.gif?sign=q-sign-algorithm%3Dsha1%26q-ak%3DAKIDYEtIenIh2OgroaBbnlidSDpMjrnvthMo%26q-sign-time%3D1727001448%3B1727002108%26q-key-time%3D1727001448%3B1727002108%26q-header-list%3Dhost%26q-url-param-list%3D%26q-signature%3D60fad023f8fff4e4f3e4d48ec8568a751c693977&)
