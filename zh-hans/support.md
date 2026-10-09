---
lang: zh-Hans
ref: support
layout: page
title: 支持
description: >
  获取 ScoreBoard for Mac 应用的帮助：报告错误、索取使用说明，
  或为你在 OBS、Streamlabs、Wirecast 或 Meld 中使用的体育记分牌提出新功能建议。
image: /img/scoreboard_for_mac_light.png
permalink: /zh-hans/support/
---

<div class="content-holder">
	<h2>ScoreBoard for Mac 应用支持</h2>

	<img class="header-image" alt="ScoreBoard for Mac 主界面" src="/img/scoreboard_for_mac_light.png">
  
	<h2>以下情况可以给开发者留言</h2>
	<ul>
		<li>解决问题（错误、故障等）</li>
		<li>获取程序使用说明</li>
		<li>提出改进需求或分享你的想法</li>
		<li>关于 ScoreBoard for Mac 应用的其他任何问题</li>
	</ul>

	<form action="https://formspree.io/f/xgernygo" method="POST">
		<label>
			<input type="email" name="_replyto" placeholder="* 你的电子邮箱" required="required">
		</label>

		<label>
			<input type="text" name="name" placeholder="你的名字">
		</label>
		
		<label>
			<textarea name="message" rows="6" placeholder="* 输入你的留言..." required="required"></textarea>
		</label>
		
		<input type="hidden" name="_subject" value="ScoreBoard support page from GitHub (zh-Hans)" />
		
		<button type="submit">发送</button>
	</form>

	<p><a href="/zh-hans/">返回 ScoreBoard for Mac</a></p>
</div>


<style>
	.header-image {
		width: 500px;
	}

	@media (prefers-color-scheme: dark) {
	  .header-image {
			content: url('/img/scoreboard_for_mac_dark.png');
	  }
	}

	input, textarea {
		width: 90%;
		padding: 10px;
		border: 1px solid #ccc;
		margin: 10px;
		font-size: 1em;
		resize: vertical;
		background-color: #ffffff;
		color: #000000;
	}

	@media (prefers-color-scheme: dark) {
		input, textarea {
			background-color: #333333;
			color: #ffffff;
			border-color: #555555;
		}
	}

	button {
		background-color: #4caf50;
		color: white;
		padding: 10px 40px;
		border: none;
		cursor: pointer;
		border-radius: 10px;
		font-size: 1.5em;
		margin: 10px;
	}

	button:hover {
		background-color: #45a049;
	}

	.content-holder {
		text-align: center;
	}

	ul {
		text-align: left;
	}

</style>
