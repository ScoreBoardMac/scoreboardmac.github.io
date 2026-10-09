---
lang: fr
ref: support
layout: page
title: Support
description: >
  Obtenez de l'aide pour l'application ScoreBoard pour Mac : signalez un bug, demandez des instructions
  ou proposez de nouvelles fonctionnalités pour votre tableau de score dans OBS, Streamlabs, Wirecast ou Meld.
image: /img/scoreboard_for_mac_light.png
permalink: /fr/support/
---

<div class="content-holder">
	<h2>Support de l'application ScoreBoard pour Mac</h2>

	<img class="header-image" alt="Écran principal de ScoreBoard pour Mac" src="/img/scoreboard_for_mac_light.png">
  
	<h2>Écrivez au développeur pour</h2>
	<ul>
		<li>Résoudre un problème (erreurs, bugs, etc.)</li>
		<li>Obtenir des instructions sur l'utilisation du programme</li>
		<li>Demander une amélioration ou proposer une idée</li>
		<li>Toute autre question sur l'application ScoreBoard pour Mac</li>
	</ul>

	<form action="https://formspree.io/f/xgernygo" method="POST">
		<label>
			<input type="email" name="_replyto" placeholder="* Votre e-mail" required="required">
		</label>

		<label>
			<input type="text" name="name" placeholder="Votre nom">
		</label>
		
		<label>
			<textarea name="message" rows="6" placeholder="* Votre message..." required="required"></textarea>
		</label>
		
		<input type="hidden" name="_subject" value="ScoreBoard support page from GitHub (fr)" />
		
		<button type="submit">Envoyer</button>
	</form>

	<p><a href="/fr/">Retour à ScoreBoard pour Mac</a></p>
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
