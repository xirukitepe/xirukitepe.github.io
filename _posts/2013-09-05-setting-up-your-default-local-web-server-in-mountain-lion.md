---
layout: post
title: "Setting up your default local web server in Mountain Lion"
description: "Learn how to magically enable the default local web server installed in your MAC OSX."
categories: Mac OSX
tags: [osx, mac, apache]
---

<h2>
	By default, there is a local web server nailed in your MAC!
</h2>
<p>
	<b>Before,</b> you can enable it via System Preferences > Sharing > Web Sharing
</p>
<p>
	<b>But,</b> things are already different since Mountain Lion. OS X Mountain Lion does not include Web Sharing as an option in the Sharing preference pane. Mountain Lion does include the Apache HTTP Server, an open-source web server (ref: <a href="https://discussions.apple.com/">Apple Discussions Forum)</a>.
</p>
<h2>How to activate Apache HTTP Server in OSX Mountain Lion?</h2>
<br/>
<img src="/assets/images/posts/apache.png" />
<br/><br/>
<p><b>First,</b> you need to create a <i>.conf</i> file in your <i>/etc/apache2/users/</i> folder.</p>
<!-- <p><pre><code>&lt;!DOCTYPE html&gt;<br/>&lt;html <b>class="fuelux"</b> lang="en"&gt;</code></pre></p>	 -->

<p>
	<strong>Run</strong> this command to create your own:
</p>

<p><pre><code>sudo pico /etc/apache2/users/username.conf</code></pre></p>

<p><b>Remember</b> that <i>username</i> is the short name of your user account:</p>

<p><b>Naturally,</b> the file will be opened in a VIM text editor.</p>

<p><b>Copy</b> the following <a href="https://gist.github.com/xirukitepe/6472728">sample configuration file</a> into your own <i>.conf</i> file. Replace the <i>/Users/xiruki/Sites/</i> path by your own path.</p>

<p><b>Make</b> sure that you already have an existing <i>Sites</i> folder inside your <i>/Users/username</i> folder</p>

<p><b>Save and Exit!</b></p>

<p><b>Open</b> your terminal and start your local web server:</p>

<p><pre><code>sudo apachectl start</code></pre></p>

<p>If you didn't encounter any errors upon starting the server, then you may now run other apachectl commands!</p>

<p>
	<ul>
		<li>sudo apachectl stop</li>
		<li>sudo apachectl restart</li>
	</ul>
</p>

<p>
	<b>Lastly,</b> you may now access your <b>http://localhost</b>.<br/>
	This is the default content of your localhost:<br/><br/>
	<img src="/assets/images/posts/it_works.png" />
</p>

<p>
	<b>To</b> access your Sites folder, go to http://localhost/~username/
</p>

<br/>
<p><b>Now you have your local web server running! Congratulations!</b></p>

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
