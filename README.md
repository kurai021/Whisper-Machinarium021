##Whisper Machinarium021

A Ghost Theme based of the default ghost theme named Casper and Whisper.

This theme is under Apache License 2.0.

###Features
- Compatiblity with Ghost 0.5.3
- Header and Footer background is configured with Blog Cover option
- Completely responsive design
- Videos responsive
- About page support
- Social buttons on header and share buttons on each post
- Code Highlighting
- Infinite scroll support
- Return to top button
- Disqus support
- Google Analytics support
- Favicon support
- 404 Error custom page
- Completely minificated (on progress)

###¿How tu setup your About page?
The about page url is "url"/about/, you only need to create a static page and configure the Post URL to about.
###Social buttons and share buttons
####On header buttons:
- Find default.hbs
- Change this section with your social accounts links and buttons
```
<ul class="social">
		<li><a href="https://www.facebook.com/richard.armuelles" target="_blank"><img src="{{asset "images/facebook.png"}}" width="48" /></a></li>
        <li><a href="https://twitter.com/raaztux" target="_blank"><img src="{{asset "images/twitter.png"}}" width="48" /></a></li>
        <li><a href="https://plus.google.com/u/0/117702515713402194890" target="_blank"><img src="{{asset "images/google.png"}}" width="48" /></a></li>
        <li><a href="https://www.linkedin.com/profile/view?id=142321855" target="_blank"><img src="{{asset "images/linkedin.png"}}" width="48" /></a></li>
        <li><a href="https://github.com/kurai021" target="_blank"><img src="{{asset "images/github.png"}}" width="48" /></a></li>
</ul>```


####On share buttons
- Find post.hbs
- Change this section with your favourite buttons, don't forget to use target="_blank" on "a" tag
```
<section class="share">
	<h4>Share this post</h4>
     <a target="_blank" href="https://twitter.com/share?text={{encode title}}&amp;url={{url absolute="true"}}">
        <img src="{{asset "images/rounded-twitter.png"}}">
     </a>
   	 <a target="_blank" href="https://www.facebook.com/sharer/sharer.php?u={{url absolute="true"}}">
       <img src="{{asset "images/rounded-facebook.png"}}">
     </a>
     <a target="_blank" href="https://plus.google.com/share?url={{url absolute="true"}}">
        <img src="{{asset "images/rounded-google.png"}}">
     </a>
 </section>```

###Code Highligting
You need to use the ```<pre>code</pre>``` method as explained on (some scripts for highlighting on specific languages already included on default.hbs) [http://alexgorbatchev.com/SyntaxHighlighter/manual/installation.html](http://alexgorbatchev.com/SyntaxHighlighter/manual/installation.html) for details

###¿Do you want to disable infinite scroll?
You only need to comment this section on default.hbs:
```<script type="text/javascript" src="{{asset "assets/jscroll/jquery.jscroll.js"}}"></script>```
```<script type="text/javascript" src="{{asset "assets/jscroll/scroll-post.js"}}"></script>```

###¿How to setup your favicon?
Copy your favicon with name "favicon.png" on assets folder
###¿How to setup Disqus?
Login on Disqus and change "var disqus_shortname = 'mightymaze'" on post.hbs with your Disqus shortname
###¿How to setup Google Analytics?
Change 'UA-48146313-1' on default.hbs with your Site ID
