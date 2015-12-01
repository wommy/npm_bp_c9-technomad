---
layout: post
published: true
category: web
---

composition start: "Wed Nov 25 2015 10:02:00 GMT-0500 (EST)"
composition end: "Wed Nov 25 2015 16:42:05 GMT-0500 (EST)"
had lunch inbetween

so [wordpress](http://wordpress.com) came out with something new a day or two ago, [Calypso!](https://developer.wordpress.com/calypso/)

i was alerted to it because of my [twitter](http://twitter.com) [highlights](https://blog.twitter.com/2015/highlighting-the-best-of-twitter-for-you) had at least 10+ tweets that some how mentioned it. i started with [techcrunch's](http://techcrunch.com/2015/11/23/wordpress-com-goes-open-source-and-gets-a-desktop-app/)

afterwards i formatted this tweet

<blockquote class="twitter-tweet" lang="en"><p lang="en" dir="ltr"><a href="https://twitter.com/hashtag/wordPress?src=hash">#wordPress</a> rewrite&#10;<a href="https://twitter.com/hashtag/calypso?src=hash">#calypso</a> <a href="https://twitter.com/hashtag/rest?src=hash">#rest</a> <a href="https://twitter.com/hashtag/api?src=hash">#api</a> <a href="https://twitter.com/hashtag/javascript?src=hash">#javascript</a> <a href="https://twitter.com/hashtag/SPA?src=hash">#SPA</a> <a href="https://twitter.com/hashtag/openSource?src=hash">#openSource</a> <a href="https://twitter.com/hashtag/github?src=hash">#github</a> <a href="https://twitter.com/hashtag/app?src=hash">#app</a> <a href="https://twitter.com/hashtag/mac?src=hash">#mac</a>&#10;<a href="https://twitter.com/hashtag/web?src=hash">#web</a> <a href="https://twitter.com/hashtag/design?src=hash">#design</a> <a href="https://twitter.com/hashtag/development?src=hash">#development</a>&#10;<a href="https://t.co/jHxGih3T4N">https://t.co/jHxGih3T4N</a></p>&mdash; Tommy Williams (@Froggie92) <a href="https://twitter.com/Froggie92/status/669282177041850368">November 24, 2015</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

i needed more information, so i went to reddit.

[this reddit comment](https://www.reddit.com/r/PHP/comments/3u44aq/regarding_wordpress/) gave some structure to calypso, but only confused me more. off to google

[this venture beat article](http://venturebeat.com/2015/11/24/wordpress-creator-matt-mullenweg-breaks-down-the-blogging-platforms-biggest-overhaul-in-years/) interviews Matt Mullenweg, CEO of [Automattic](automattic.com), wordpress's parent company: they spent 20 months on redoing everything in javascript, but then clarifies that it was only the front end ui and that the back end is still all php; about wordpresses relevancy, more like hegemony; interviewer brings up rivals like [medium](https://medium.com/), which i personally enjoy; linux / windows support. overall blah article. 

afterwhich i fired off this tweet

<blockquote class="twitter-tweet" lang="en"><p lang="en" dir="ltr">not looking forward to learning <a href="https://twitter.com/hashtag/wordpress?src=hash">#wordpress</a>&#39;s new <a href="https://twitter.com/hashtag/calypso?src=hash">#calypso</a>&#10;relevance =/= avoiding death &#10;<a href="https://twitter.com/hashtag/web?src=hash">#web</a> <a href="https://twitter.com/hashtag/design?src=hash">#design</a> <a href="https://twitter.com/hashtag/development?src=hash">#development</a></p>&mdash; Tommy Williams (@Froggie92) <a href="https://twitter.com/Froggie92/status/669284822087434240">November 24, 2015</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

if you could not tell, i still didnt know what it was about really, so i did a bunch more digging.

[more reddit comments](https://www.reddit.com/r/learnprogramming/comments/3u3qoo/about_changes_on_wordpress/): admin ui change, got it already.

finally upon [/r/wordpress](http://reddit.com/r/wordpress) (which i do not subscribe to) and opened up a bunch of tabs:

[reddit](https://www.reddit.com/r/Wordpress/comments/3u34pc/thoughts_on_calypso/) & [original article](http://blog.versionpress.net/2015/11/thoughts-on-calypso/)

first, the reddit comments are bland. they congradulate automattic, emphasizing the split between front end user interfaces and backend powered wordpress, which further gives weight to a trend that i've been seeing for a couple years now. wordpress's admin interface is a blessing and a curse: it set the stage for admin UIs but its lack of workflow customizability has spawned dozens of spinoffs that 'do it better', a strange spot to be in. hopefully this calypso really gives some power to areas that need it.

the actual article doesnt really say much. he talks about a wp-cli, which my workings in node has revealed the immense benefit of, but i already got that from the techcrunch article. Trac => Github + SVN => Git, cool. he brings up [react](https://facebook.github.io/react/), which the techcrunch article does not mention, which only raises more questions. towards the bottom he really highlights this, mentioning all those misinformed tweets. 

when i saw javascript in the techcrunch article, i was happy. they even mentioned wordpress moving away from my two major annoyances, php and mysql! but this isnt the case.

finally upon'd [matt's own blog post about calypso and the update](http://ma.tt/2015/11/dance-to-calypso/). starts with some finance; moves to sprawling codebase; drops that 25% of the web runs on wordpress; needing a huge improvement: 20x not 2x = CALYPSO: Node and React; 100% API-powered; social, responsive, authoring, multi-site managing, jetpack plugins, 100% open source. Sites linux release cycle; buncha explore links; reiterates that the 25% that use wordpress should be proud of open source; wraps with an infograph highlighting changes.

should have started with this one! finally a juicy article! okay so some critical anaylsis: he blows out some financial numbers at the beginning, which is totally CEO's job, before he jumps into calypso. ive worked off and on with wordpress and other lamp stacks for a few years now and i've never had a good time with it; maybe it was because i was trained in ruby and rails. specifically trying to troubleshoot wordpress core was major problem, which calypso doesnt touch upon at all. thats fine, im glad i know and understand that. but i think WP's front end UI fork of node and react speaks to contemporary technologies. when i start a project, i start it in node. when clients ask for a lamp stack, im very dubious: either its legacy code, which i really dont want to get muddled in, or they are uninformed. dont get me wrong, LAMP paved the web's road: most of the actions/events/words/phrases/ideas that designers/developers brew were first done in php, and usually thats still the most efficient way to achieve those goals. im not trying to get into php critiques, as that could be a whole separate blog post, but its been 10 years since 2005, we have more verbose tools now. yes you need to know where you came from / how things work but you also need to be able to keep up with the pack. react is the pack today. react is bleeding edge. i havent worked much with react other than a few tutorials, but i already see its benefit. the face that wordpress sculpted this whole front end ui in it speaks to its potential. 

other parts of this update seem to be blown to the wayside in this update. yeah you have a mac native app, big whoop. with react, the web interface is operating at as close to native speeds as possible, another huge benefit / selling point of react. yeah it has notifications, which are cool, but react can do that too. API's are great, but WP should have already had that for tech savvy admins. open source is a huge move too, with their port to github; i am most familiar with github, and i believe most people are. IMHO, one of WP's biggest drawbacks is having to sculpt a bunch of middleware to get what you want, but with github, thats as easy as creating a fork of calypso, and then forking that for new projects. now if wordpress would only port their backend, which i doubt will happen for some time, if ever.

things i would like to see next:
command line tools: yeah, wordpress has all these cool tools, but the UI hides them. i want to add seven menu items, hell i want to import a menu from elsewhere; whys that so hard, where are the docs on that.
better doc integration: the WP should be the starting point, with [stackoverflow](http://stackoverflow.com) as the backup, but docs are so messy they raise more questions than they answer; fix plz!

the infograph at the bottom is lame / could be so much better.

but i cant wait to dig thru his links at the bottom, but that in itself has to be another post. next article

i found this [video](https://videopress.com/v/bi7dnCzS) in a reddit comment somewhere. its got some useful information, a tl;dr of above sources.

my problem with WP: they give people this admin panel which gives anyone all the tools to create and maintain a blog. yet i find that most people just want to focus on the content and dont want to maintain it themselves. but wordpress thought of this and allows delegation of admin privileges, yet didn't think to give admins a secondary layer of tools. ill admit: i havent dug into automattic's peripheral tools like jetpack, but i dont think i should have to. as a developer, i dont want to have to learn as entire ecosystem, especially one as focused on blog publishing. yeah yeah, they may power 25% of the web, but is that such a boasting point if they do it poorly? 

What i will give WP: I have based my own development workflow around WP. I use <prose.io> which simplistically is a WP admin panel for [Jekyll](http://jekyllrb.com). In the above video, I like their photo gallery widget to the point that im probably going to steal it and use a variant for my own website platform. They are the biggest / forerunner. they have succeeded in democratizing online publishing. and while I am glad they are clinging to relevance, eventually all things need to die. Calypso seems like an attempt to breathe life into WP, and while it definitely is on the right path, i think its too little too late. ill revisit whenever they create a Node to PHP transpiler, when there is a noSQL backend option. MEAN stacks arent that new, especially when compared to React. as always, im hopeful; if anyone could modernize web publishing, its WP.

TODO on this blogpost:

- split rants into wordpress / calypso
- be more consise/efficient in displaying/conveying my search process
- jot notes, instead of recall

FURTHE[R]EADING (shit i didnt even get to) :

- <https://developer.wordpress.com/calypso/>
    - <https://github.com/Automattic/wp-calypso>
- <http://jetpack.me/>
- rewatch video / explore calypso for ideas
- <https://www.reddit.com/r/Wordpress>
- <https://www.reddit.com/r/Wordpress/comments/3u44rt/calypso_php_and_js_discussion/>
- <https://www.reddit.com/r/Wordpress/comments/3tyuu6/welcome_to_the_new_wordpresscom_and_wordpresscom/>
- <https://en.blog.wordpress.com/2015/11/23/the-new-wordpress-dot-com/>
- <https://twitter.com/search?q=wordpress%20calypso&src=typd>
- <https://www.reddit.com/r/PHP/comments/3u44aq/regarding_wordpress/>
