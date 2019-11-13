---
layout: page
title: Permissions
show_tile: true
---
    
<!-- Main -->
<div id="main" class="alt">

<!-- One -->
<section id="one">
	<div class="inner">
		<header class="major">
			<h1>{{ page.title }}</h1>
		</header>
		{% if page.image %}<span class="image main"><img src="{{ site.baseurl }}/{{ page.image }}" alt="" /></span>{% endif %}
		<p>In a nutshell, BibleBot requires the following permissions: <code>Read Messages</code>, <code>Send Messages</code>, <code>Read Message History</code>, <code>Manage Messages</code>, <code>Embed Links</code>, <code>Add Reactions</code>.</p>
    <p>Here's a list of the reasons why this is needed (screenshots will be added later):
      <ul>
        <li>Read Messages - The bot can't see the channel unless this is available.</li>
        <li>Send Messages - The bot will not be able to respond to any messages without it.</li>
	      <li>Read Message History - This is necessary for paged commands like <code>+search</code>, <code>+versions</code>, <code>+biblebot</code>, or any of the extrabiblical content. If this isn't provided, BibleBot won't be able to detect changes to the page properly.</li>
        <li>Manage Messages - This is necessary after paged commands timeout, so BibleBot can remove the reactions. BibleBot removes the reactions at the timeout to indicate that further interaction requires you to redo the command.</li>
        <li>Embed Links - Despite the fact that BibleBot does not use a lot of links, this permission allows you to see BibleBot in the fancy boxes that you know and love.</li>
        <li>Add Reactions - As aforementioned, BibleBot needs to be able to add reactions for the paged commands, otherwise they will not function.</li>
      </ul>
    </p>
  <p><b>If you're encountering permissions issues, the quickest option is to kick the bot from your server and reinvite it using the proper invite link. Click <a href="https://discordapp.com/oauth2/authorize?client_id=361033318273384449&scope=bot&permissions=93248">here</a> to invite the bot.</b></p>
  
	</div>
</section>

</div>
