---
lang: de
ref: support
layout: page
title: Support
description: >
  Hilfe zur App ScoreBoard für Mac: Fehler melden, Anleitungen anfordern
  oder neue Funktionen für dein Sport-Scoreboard in OBS, Streamlabs, Wirecast oder Meld vorschlagen.
image: /img/scoreboard_for_mac_light.png
permalink: /de/support/
---

<div class="content-holder">
	<h2>Support für die App ScoreBoard für Mac</h2>

	<img class="header-image" alt="Hauptfenster von ScoreBoard für Mac" src="/img/scoreboard_for_mac_light.png">
  
	<h2>Schreib dem Entwickler, wenn du</h2>
	<ul>
		<li>Ein Problem lösen möchtest (Fehler, Abstürze usw.)</li>
		<li>Eine Anleitung zur Nutzung des Programms brauchst</li>
		<li>Eine Verbesserung wünschst oder eine Idee vorschlagen möchtest</li>
		<li>Ein anderes Anliegen zur App ScoreBoard für Mac hast</li>
	</ul>

	<form action="https://formspree.io/f/xgernygo" method="POST">
		<label>
			<input type="email" name="_replyto" placeholder="* Deine E-Mail" required="required">
		</label>

		<label>
			<input type="text" name="name" placeholder="Dein Name">
		</label>
		
		<label>
			<textarea name="message" rows="6" placeholder="* Deine Nachricht..." required="required"></textarea>
		</label>
		
		<input type="hidden" name="_subject" value="ScoreBoard support page from GitHub (de)" />
		
		<button type="submit">Senden</button>
	</form>

	<p><a href="/de/">Zurück zu ScoreBoard für Mac</a></p>
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
