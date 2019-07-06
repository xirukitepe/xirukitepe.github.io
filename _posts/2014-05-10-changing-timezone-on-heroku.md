---
layout: post
title: "Changing Timezone on Heroku"
description: "Discover how to change timezone on the Heroku Cedar stack. Time is gold!"
categories: Cloud Service
tags: [heroku, cloud]
---

<h2>
	Howdy! I know you're here because you're a <code>Heroku</code> fan or a forced <code>Heroku</code> user.
</h2>
<p>
	<b>Well,</b> it's not a big deal though.
</p>
<p>
	<b>Honestly,</b> I really like how you can wrap up things quickly via Heroku. Heroku's automation is way bitcher than bitch. I'm a fan, YES! But it's not that I can always afford their sky-high packages.
</p>
<p>
	<b>So much about it,</b> I'll shut my mouth now before a Heroku spy learns everything about me. I want to live longer, you know.
</p>
<h2>What is a timezone?</h2>
<br/>
<img src="/assets/images/posts/timezone.png" />
<br/><br/>
<p><b>Timezone,</b> is a region that has a uniform standard time for legal, commercial, and social purposes. It is convenient for areas in close commercial or other communication to keep the same time, so time zones tend to follow the boundaries of countries and their subdivisions.</p>
<!-- <p><pre><code>&lt;!DOCTYPE html&gt;<br/>&lt;html <b>class="fuelux"</b> lang="en"&gt;</code></pre></p>	 -->

<p>
	<strong>By the way,</strong> thanks to <a href="http://en.wikipedia.org/wiki/Time_zone"><i>Wikipedia</i></a>, for the oh-so-meaningful meaning of <a href="http://en.wikipedia.org/wiki/Time_zone"><b>Timezone</b></a>.
</p>

<h2>What do you need before changing timezone on Heroku Cedar stack?</h2>

<p><b>Appropriate Timezone Name String?</b> That sounds weird?</p>

<p><b>First,</b> you really need to know your desired appropriate zone name string.</p>

<p><b>Search</b> for your desired zone name string <a href="http://en.wikipedia.org/wiki/List_of_tz_database_time_zones"><b>here</b></a>.</p>

<p><b>Second,</b> open your console/shell so that you could perform the command needed in changing the timezone.</p>

<p><b>Example,</b> my zone name string is America/Vancouver</p>

<p><b>Simply</b> run this command:</p>

<p><pre><code>heroku config:add TZ=America/Vancouver</code></pre></p>

<p>Your Heroku app will restart after!</p>
<br/><br/>
<p>
	<b>Oh well,</b> you can check/test if it's really working by performing the ff:<br/>
</p>

<p>
	<b>In console/shell, run:</b>
</p>

<p><pre><code>heroku run console</code></pre></p>

<p><b>Then,</b> check the time:</p>

<p><pre><code>Time.now</code></pre></p>

<br/>
<br/>

<p><b>That should be all set for you!</b></p>

<!-- Twitter -->
<script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0];if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src="//platform.twitter.com/widgets.js";fjs.parentNode.insertBefore(js,fjs);}}(document,"script","twitter-wjs");</script>

<!-- Google + -->
<script type="text/javascript">
  (function() {
    var po = document.createElement('script'); po.type = 'text/javascript'; po.async = true;
    po.src = 'https://apis.google.com/js/plusone.js';
    var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(po, s);
  })();
</script>
