---
lang: es
ref: support
layout: page
title: Soporte
description: >
  Obtén ayuda con la app ScoreBoard para Mac: informa de errores, solicita instrucciones
  o sugiere nuevas funciones para tu marcador deportivo en OBS, Streamlabs, Wirecast o Meld.
image: /img/scoreboard_for_mac_light.png
permalink: /es/support/
---

<div class="content-holder">
	<h2>Soporte de la app ScoreBoard para Mac</h2>

	<img class="header-image" alt="Pantalla principal de ScoreBoard para Mac" src="/img/scoreboard_for_mac_light.png">
  
	<h2>Escribe al desarrollador para</h2>
	<ul>
		<li>Resolver un problema (errores, fallos, etc.)</li>
		<li>Recibir instrucciones sobre cómo usar el programa</li>
		<li>Pedir mejoras o proponer tu idea</li>
		<li>Cualquier otra consulta sobre la app ScoreBoard para Mac</li>
	</ul>

	<form action="https://formspree.io/f/xgernygo" method="POST">
		<label>
			<input type="email" name="_replyto" placeholder="* Tu correo electrónico" required="required">
		</label>

		<label>
			<input type="text" name="name" placeholder="Tu nombre">
		</label>
		
		<label>
			<textarea name="message" rows="6" placeholder="* Escribe tu mensaje..." required="required"></textarea>
		</label>
		
		<input type="hidden" name="_subject" value="ScoreBoard support page from GitHub (es)" />
		
		<button type="submit">Enviar</button>
	</form>

	<p><a href="/es/">Volver a ScoreBoard para Mac</a></p>
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
