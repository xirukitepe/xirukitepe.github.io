---
layout: post
title: "Installing Phonegap in MAC OSX"
description: "Instant information with a snap, on how to install Phonegap in your MAC OSX. Start creating awesome mobile applications via Phonegap."
categories: Mobile Development
tags: [mobile, phonegap]
---

<h2>
	Start creating awesome mobile applications using this technology!
</h2>
<p>
	<a href="http://phonegap.com/">Phonegap</a> is an open source framework for quickly building cross-platform mobile apps using HTML5, Javascript and CSS. It supports various platforms such as...
</p>
<p>
	<ul>
		<li>IOS</li>
		<li>Android</li>
		<li>Blackberry OS</li>
		<li>WebOS</li>
		<li>Windows</li>
		<li>Symbian</li>
		<li>Bada</a>
	</ul>
</p>
<h2>How to install Phonegap in MAC OSX?</h2>
<br/>
<img src="/assets/images/posts/phonegap.png" />
<br/><br/>
<p><b>First,</b> you need to install <a href="http://nodejs.org/">Node JS</a> and <a href="https://npmjs.org/">NPM (Node Package Modules)</a>. We can achieve those via <a href="http://brew.sh/">Homebrew</a>, the missing package manager for OS X. </p>
<!-- <p><pre><code>&lt;!DOCTYPE html&gt;<br/>&lt;html <b>class="fuelux"</b> lang="en"&gt;</code></pre></p>	 -->

<p>
	<strong>Install</strong> Homebrew via this command:
</p>

<p><pre><code>ruby -e "$(curl -fsSL https://raw.github.com/mxcl/homebrew/go)"</code></pre></p>

<p><b>After</b> installing Homebrew, follow the generated instructions!</p>

<p><b>Make</b> sure that once you run the <b>`brew doctor`</b> command, everything is fine and no warnings are executed.</p>

<p>Once Homebrew is setup correctly, it's time to install Node JS via brew!</p>

<p><pre><code>brew install node</code></pre></p>

<p><b>Then,</b> install NPM...</p>

<p><pre><code>curl https://npmjs.org/install.sh | sh</code></pre></p>

<p><b>Finally,</b> it's time for you to install Phonegap all the way!</p>

<p><pre><code>sudo npm install -g phonegap</code></pre></p>

<p>For more info: <a href="http://phonegap.com/install/">Check it here!</a></p>

<br/>
<p><b>I'll be posting a sample tutorial on how to use Phonegap soon! So wait for it!</b></p>

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
