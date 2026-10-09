---
lang: ru
ref: support
layout: page
title: Поддержка
description: >
  Помощь по приложению ScoreBoard для Mac: сообщите об ошибке, запросите инструкцию
  или предложите новую функцию для спортивного табло в OBS, Streamlabs, Wirecast или Meld.
image: /img/scoreboard_for_mac_light.png
permalink: /ru/support/
---

<div class="content-holder">
	<h2>Поддержка приложения ScoreBoard для Mac</h2>

	<img class="header-image" alt="Главный экран ScoreBoard для Mac" src="/img/scoreboard_for_mac_light.png">
  
	<h2>Напишите разработчику, если нужно</h2>
	<ul>
		<li>Решить проблему (ошибки, сбои и т. п.)</li>
		<li>Получить инструкции по работе с программой</li>
		<li>Попросить доработку или предложить свою идею</li>
		<li>По любому другому вопросу о приложении ScoreBoard для Mac</li>
	</ul>

	<form action="https://formspree.io/f/xgernygo" method="POST">
		<label>
			<input type="email" name="_replyto" placeholder="* Ваш e-mail" required="required">
		</label>

		<label>
			<input type="text" name="name" placeholder="Ваше имя">
		</label>
		
		<label>
			<textarea name="message" rows="6" placeholder="* Введите сообщение..." required="required"></textarea>
		</label>
		
		<input type="hidden" name="_subject" value="ScoreBoard support page from GitHub (ru)" />
		
		<button type="submit">Отправить</button>
	</form>

	<p><a href="/ru/">Вернуться к ScoreBoard для Mac</a></p>
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
