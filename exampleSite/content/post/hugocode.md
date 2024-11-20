+++
author = "爸比娃娃"
title = "一些 hugo 短代码"
date = "2024-11-20"
tags = [
    "网站制作",
]

+++

{\{< notice notice-warning >}}本文为了防止在代码块中的短代码被 Hugo 转译，在代码块中添加了 \，请在使用时去除{\{< notice >}}

## notice

```go
{\{< notice notice-warning >}}
你好。
{\{< /notice >}}

{\{< notice notice-info >}}
你好。
{\{< /notice >}}

{\{< notice notice-note >}}
你好。
{\{< /notice >}}

{\{< notice notice-tip >}}
你好。
{\{< /notice >}}
```

Copy

预览：



你好。



## 隐藏内容

```fallback
{\{< detail "点这里看隐藏内容！" >}}
这里是隐藏内容！🥰
{\{< /detail >}}
```

Copy

预览：

<details style="box-sizing: border-box; scrollbar-width: auto; scrollbar-color: var(--scrollbar-thumb)transparent; display: block; color: rgb(58, 58, 58); font-family: fontello, sans-serif; font-size: 18px; font-style: normal; font-variant-ligatures: normal; font-variant-caps: normal; font-weight: 400; letter-spacing: normal; orphans: 2; text-align: start; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; white-space: normal; background-color: rgb(243, 243, 238); text-decoration-thickness: initial; text-decoration-style: initial; text-decoration-color: initial;"><summary style="box-sizing: border-box; scrollbar-width: auto; scrollbar-color: var(--scrollbar-thumb)transparent; display: list-item;">点这里看隐藏内容！</summary></details>



## 聊天气泡

```bash
{\{< chat position="left" name="John Doe" timestamp="2023-09-12 14:30">}}
这是左边的消息内容。
{\{< /chat >}\}

{\{< chat position="right" name="Alice" timestamp="2023-09-12 14:45" >}} 
这是右边的消息内容，测试长长长长长长长长长长长长长长长长长长长长长长长长度。
{\{< /chat >}\}
```

Copy

预览：

John Doe  2023-09-12 14:30

这是左边的消息内容。



2023-09-12 14:45  Alice

这是右边的消息内容，测试长长长长长长长长长长长长长长长长长长长长长长长长度。

## 时间轴

```fallback
{\{< timeline date="2023-10-01" title="国庆节" description="祖国生日快乐" tags="节日" url="" >}\}
```

Copy

预览：

2023-10-01

节日

国庆节

祖国生日快乐



## 播放视频

哔哩哔哩

```bash
{\{< bilibili VIDEO_ID PART_NUMBER >}\}
```

Copy

提示：



Video_ID: AV 或 BV PART_NUMBER（可选）：指定要播放的视频序号



<iframe src="https://player.bilibili.com/player.html?as_wide=1&amp;high_quality=1&amp;page=1&amp;bvid=BV1wT421v7ZN" scrolling="no" frameborder="no" framespacing="0" allowfullscreen="" style="box-sizing: border-box; scrollbar-width: auto; scrollbar-color: var(--scrollbar-thumb)transparent; width: 883.25px; height: 463.078px; left: 0px; top: 0px; border: 0px;"></iframe>

腾讯

```fallback
{{\< tencent g0014r3khdw >}}
```

Copy

预览：

<iframe src="https://v.qq.com/txp/iframe/player.html?vid=g0014r3khdw&amp;auto=0" scrolling="no" frameborder="no" framespacing="0" allowfullscreen="" style="box-sizing: border-box; scrollbar-width: auto; scrollbar-color: var(--scrollbar-thumb)transparent; width: 883.25px; height: 463.078px; left: 0px; top: 0px; border: 0px;"></iframe>



YouTube 视频

```fallback
{{\< youtube VIDEO_ID >}}
```

Copy

通用视频文件



VIDEO_URL 可以是 URL 或相对于 static 目录的路径。例如， src="/video/my-video.mp4" 将嵌入站点文件夹的视频文件 static/video/my-video.mp4 。

autoplay 属性是可选的。它可用于指定是否应自动播放视频。 poster 属性是可选的。它可用于指定视频的海报图像。



```fallback
{{\< video VIDEO_URL >}}

{{\< video src="VIDEO_URL" autoplay="true" poster="./video-poster.png" >}}
```