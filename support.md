---
layout: page
title: Support
permalink: /support/
---

<div class="content-holder">
	<h2>ScoreBoard Mac app support</h2>

	<img class="header-image" alt="Scoreboard for mac Main Screen" src="/img/scoreboard_for_mac_light.png">
  
	<h2>Send a message to the developer for</h2>
	<ul>
		<li>Problem solving (errors, bugs, etc.)</li>
		<li>Receiving instructions on how to use the program</li>
		<li>Request improvements or suggest your idea</li>
		<li>Any other reasons for the ScoreBoard for Mac app</li>
	</ul>

	<form action="https://formspree.io/f/xgernygo" method="POST">
		<label>
			<input type="email" name="_replyto" placeholder="* Your e-mail" required="required">
		</label>

		<label>
			<input type="text" name="name" placeholder="Your name">
		</label>
		
		<label>
			<textarea name="message" rows="6" placeholder="* Type your message..." required="required"></textarea>
		</label>
		
		<input type="hidden" name="_subject" value="ScoreBoard support page from GitHub" />
		
		<button type="submit">Send</button>
	</form>
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
