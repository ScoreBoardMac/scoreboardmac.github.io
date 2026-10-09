---
lang: zh-Hans
ref: home
title: 适用于 OBS、Streamlabs、Wirecast 和 Meld 的记分牌
description: >
  可免费试用的 macOS 记分牌应用，支持 OBS、Streamlabs、Wirecast 和 Meld。通过简单的 TXT 文件叠加，
  在体育直播中实时显示比分、计时器、罚时和球队统计数据。
image: /img/scoreboard_for_mac_light.png
layout: home
permalink: /zh-hans/
---

一款功能完整的工具，可在 OBS、Streamlabs、Wirecast、Meld 以及其他支持文本文件或图像文件来源的直播软件中显示体育直播的统计数据。它能帮助你在在线体育直播画面上叠加显示某场比赛所需的统计信息。

文本数据会写入电脑磁盘上的 TXT 文件（默认保存在“下载”文件夹）。每个文件都可以在直播软件中添加为来源（来源：文本），并叠加在你的记分牌图片上。

<p align="center">
	<img class="header-image" alt="ScoreBoard for Mac 主界面" src="/img/scoreboard_for_mac_light.png">
</p>

## 记分牌可以在体育直播中显示：
- 时间（倒计时或正计时），精确到十分之一秒
- 带两个预设的附加计时器（例如用于篮球）
- 每支球队的进球（得分、射门）
- 两支球队各两个附加得分/射门计数器
- 比赛阶段（半场、节）
- 两支球队及比赛的名称
- 两支球队及比赛的描述/状态/宣传内容
- 冰球及类似运动的罚时及其计时器
- 足球的黄牌和红牌
- 两支球队及比赛的队徽和宣传图

### 其他功能：
- 便捷操控的快捷键
- 交换两队统计数据
- 重置统计数据
- 自动保存记分牌设置
- 可选择 TXT 输出文件的保存目录
- 可按 +1、+2、+3 增加比分
- 可设置进球计数的增量
- 支持触控栏（Touch Bar）操控
- 可为比赛阶段添加后缀（1st、2nd、3rd）
- 比分可补零显示（01 – 05）

第一次使用？请按照分步[设置指南](/zh-hans/guides/)在 OBS 中添加你的第一个记分牌。

## 用户评价

_评价保留英文原文。_

NP2003 | djithm | TofuDunk | tiivonen
--- | --- | --- | ---
I've been using this program since it was v1.0 on the OBS Forums - this is a fantastic program. | Excellent application that has all the tools required to use for your score bug in OBS. So much better than some of the paid subscriptions as long as you have the ability to create your own graphics for the scoreboard portion. Keep up the great work and I look forward to your updates! | This app has made it much easier for me to keep score during my board game streaming sessions. | Simple and easy to use. I use it for floorball streaming. Original M1 mbpro handles scoreboard and streaming 1080p 50p around 10% CPU usage.

<p align="center">
    <a href="https://apps.apple.com/app/id1579159150" title="在 Mac App Store 下载">
        <img alt="在 Mac App Store 下载" src="/img/MacAppStore.png">
    </a>
</p>

## ScoreBoard 免费版
**免费版**供试用：[下载](/free-apps/ScoreBoard-free.zip)后解压，将应用移到“应用程序”文件夹即可。  
免费版功能完整，但部分字段的文本输出受到限制。  
_已通过 Apple 公证和验证，可放心在 Mac 上下载和使用。_
<p align="center">
    <a href="/free-apps/ScoreBoard-free.zip" title="免费下载试用版">
        <img alt="免费下载试用版" src="/img/free-download.png">
    </a>
</p>

## ScoreBoard 和 OBS 截图
<p align="center">
  {% include screenshot.html name="1_main" alt="ScoreBoard for Mac 主界面，包含比分和计时器控制" %}
  <br>
  {% include screenshot.html name="2_preferences" alt="ScoreBoard for Mac 偏好设置，用于自定义记分牌输出" %}
  <br>
  {% include screenshot.html name="3_hotkeys" alt="ScoreBoard for Mac 的快捷键和触控栏操作" %}
  <br>
  {% include screenshot.html name="4_txtFiles" alt="ScoreBoard for Mac 输出的 TXT 文件在 OBS 中用作文本来源" %}
  <br>
</p>

## 视频教程
_此后 OBS 和 ScoreBoard 已多次更新，但视频中的设置基本相同。视频为英文。_

<div class="video-container">
  <iframe src="https://www.youtube.com/embed/dHj56FIE2ng?si=q62r_uccgddo2KXv&start=50" allowfullscreen></iframe>
</div>


## 在 OBS 中设置完成后的记分牌示例
<p align="center">
	<img width="800" alt="OBS 中的记分牌模板示例" src="/img/output_example.jpg">
</p>

## 常见问题

**ScoreBoard 支持 Streamlabs、Wirecast 和 Meld 吗？**  
支持。ScoreBoard 会把比分、计时器和统计数据写入磁盘上的 TXT 文件（宣传图和队徽写入图像文件）。任何支持文本文件或图像文件来源的直播软件——包括 OBS、Streamlabs、Wirecast 和 Meld——都可以读取并以叠加层形式显示。

**有免费版吗？**  
有。可以下载[免费试用版](/free-apps/ScoreBoard-free.zip)，已通过 Apple 公证和验证。它功能完整，只是部分字段的输出受限。完整版可在 [Mac App Store](https://apps.apple.com/app/id1579159150) 获取。

**ScoreBoard 以什么格式输出数据？**  
文本值（比分、计时器、球队名称等）输出为纯 TXT 文件，球队/比赛队徽和宣传图输出为图像文件。你在应用中操控比赛时，这些文件会自动更新。

**ScoreBoard 需要联网或注册账号吗？**  
不需要。ScoreBoard 完全在你的 Mac 本地运行，不收集任何数据——详见[隐私政策](/zh-hans/privacy/)。

## 其他
[隐私政策](/zh-hans/privacy/)

[联系支持](/zh-hans/support/)\
*欢迎反馈错误、提出需求和问题。*

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "SoftwareApplication",
  "name": "Sports Scoreboard for OBS",
  "description": "为 OBS、Streamlabs、Wirecast、Meld 等软件提供带记分牌统计数据的体育直播。",
  "inLanguage": "zh-Hans",
  "url": "https://scoreboardmac.github.io/zh-hans/",
  "applicationCategory": "MultimediaApplication",
  "operatingSystem": "macOS",
  "offers": {
    "@type": "Offer",
    "price": "9.99",
    "priceCurrency": "USD",
    "url": "https://apps.apple.com/app/id1579159150"
  },
  "aggregateRating": {
    "@type": "AggregateRating",
    "ratingValue": "4.5",
    "reviewCount": "44"
  },
  "review": [
    {
      "@type": "Review",
      "author": { "@type": "Person", "name": "NP2003" },
      "reviewBody": "I've been using this program since it was v1.0 on the OBS Forums - this is a fantastic program."
    },
    {
      "@type": "Review",
      "author": { "@type": "Person", "name": "djithm" },
      "reviewBody": "Excellent application that has all the tools required to use for your score bug in OBS. So much better than some of the paid subscriptions as long as you have the ability to create your own graphics for the scoreboard portion. Keep up the great work and I look forward to your updates!"
    },
    {
      "@type": "Review",
      "author": { "@type": "Person", "name": "TofuDunk" },
      "reviewBody": "This app has made it much easier for me to keep score during my board game streaming sessions."
    },
    {
      "@type": "Review",
      "author": { "@type": "Person", "name": "tiivonen" },
      "reviewBody": "Simple and easy to use. I use it for floorball streaming. Original M1 mbpro handles scoreboard and streaming 1080p 50p around 10% CPU usage."
    }
  ]
}
</script>

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "inLanguage": "zh-Hans",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "ScoreBoard 支持 Streamlabs、Wirecast 和 Meld 吗？",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "支持。ScoreBoard 会把比分、计时器和统计数据写入磁盘上的 TXT 文件（宣传图和队徽写入图像文件）。任何支持文本文件或图像文件来源的直播软件——包括 OBS、Streamlabs、Wirecast 和 Meld——都可以读取并以叠加层形式显示。"
      }
    },
    {
      "@type": "Question",
      "name": "有免费版吗？",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "有。可以下载免费试用版，已通过 Apple 公证和验证。它功能完整，只是部分字段的输出受限。完整版可在 Mac App Store 获取。"
      }
    },
    {
      "@type": "Question",
      "name": "ScoreBoard 以什么格式输出数据？",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "文本值（比分、计时器、球队名称等）输出为纯 TXT 文件，球队/比赛队徽和宣传图输出为图像文件。你在应用中操控比赛时，这些文件会自动更新。"
      }
    },
    {
      "@type": "Question",
      "name": "ScoreBoard 需要联网或注册账号吗？",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "不需要。ScoreBoard 完全在你的 Mac 本地运行，不收集任何数据。"
      }
    }
  ]
}
</script>

<!--Styles-->
<style>
	.header-image {
		width: 500px;
	}

	@media (prefers-color-scheme: dark) {
	  .header-image {
			content: url('/img/scoreboard_for_mac_dark.png');
	  }
	}
	
	.video-container {
		width: 100%;
		max-width: 720px;
		margin: 0 auto;
	}

	.video-container iframe {
		width: 100%;
		aspect-ratio: 4/3; /* или 16/9 для широкоформатных видео */
		border: none;
	}
</style>
