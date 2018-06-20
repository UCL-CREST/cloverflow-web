---
title: Open Comments & Discussions
permalink: /docs/discussions/
---

## Open Comments

We also invited the Answerers survey's participants to give a
free-form comment regarding their concerns of answering Stack Overflow with code
snippets. Besides the one we present earlier in the introduction, these are
interesting comments we received.

<div class="panel panel-info">
    <div class="panel-heading">
        <h3 class="panel-title">Comment 1</h3>
    </div>
    <div class="panel-body">
    The real issue is less about the amount the code snippets
    	on SO than it is about the staggeringly high number of software
    	professionals that mindlessly use them without understanding what they're
    	copying, and the only slightly less high number of would-be professionals that
    	post snippets with built-in security issues.  A related topic is beginners who
    	post (at times dangerously) misleading tutorials online on topics they actually
    	know very little about. Think PHP/MySQL tutorials written 10+ years after
    	<code class="highlighter-rouge">mysql_*</code> functions were obsolete, or the recent regex tutorial that
    	got posted the other day on HackerNew
      (<a href="https://news.ycombinator.com/item?id=14846506">https://news.ycombinator.com/item?id=14846506</a>). They're also full of
    	toxic code snippets.
    </div>
</div>

<div class="panel panel-info">
    <div class="panel-heading">
        <h3 class="panel-title">Comment 2</h3>
    </div>
    <div class="panel-body">
    When I copy code it's usually short enough to be considered "fair
    		use" but I am not a lawyer or copyright expert so some guidance from Stack Overflow would be
    		helpful. I'd also like the ability to flag/review questions that violate these
    		guidelines.
    </div>
</div>

<div class="panel panel-info">
    <div class="panel-heading">
        <h3 class="panel-title">Comment 3</h3>
    </div>
    <div class="panel-body">
    My only concern, albeit minor, is that I know people blindly copy
    		my code without even understanding what the code does.
    </div>
</div>

<div class="panel panel-info">
    <div class="panel-heading">
        <h3 class="panel-title">Comment 4</h3>
    </div>
    <div class="panel-body">
    The main problem for me/us is outdated code, esp. as old answers
    		have high google rank so that is what people see first, then try and fail. Thats
    		why we're moving more and more of those examples to knowledge base and docs and
    		rather link to those.
    </div>
</div>

<div class="panel panel-info">
    <div class="panel-heading">
        <h3 class="panel-title">Comment 5</h3>
    </div>
    <div class="panel-body">
    Lot of the answers are from hobbyist so the quality is poor.
    		Usually they are hacks or workarounds (even MY best answer on Stack Overflow is a
    		workaround).
    </div>
</div>

## Discussions

Our study discovers links from code in open source projects to code snippets on
Stack Overflow using clone detection techniques. These links enable us to
discover toxic code snippets with outdated code or licensing problems.
The links can be exploited further to mitigate the problems of reusing outdated online clones and
incompatible license on Stack Overflow code snippets. We propose the following
actionable items:

<div class="panel panel-primary">
    <div class="panel-heading">
        <h3 class="panel-title">Preventive measure</h3>
    </div>
    <div class="panel-body">
    We encourage Stack Overflow to enforce attribution when source code snippets have
    	been copied <b>from</b> licensed software projects to Stack Overflow. Moreover, an
    	IDE plug-in that can automatically detect pasted source code and follow the link
    	to Stack Overflow and then to the original open source projects, could also
    	prevent the issue of license violation.
    </div>
</div>

<div class="panel panel-primary">
    <div class="panel-heading">
        <h3 class="panel-title">Detective measure</h3>
    </div>
    <div class="panel-body">
    A system to detect outdated source code snippets on Stack Overflow is needed. The
  	system can leverage the online clone detection techniques in this study to
  	periodically check if the cloned snippets are still up-to-date with their
  	originals.
  	With such a system, the poster can be notified when the code has been updated
  	in the original project so that he/she can update their code on Stack Overflow
  	accordingly. On the other hand, with a crowdsourcing solution using an IDE
  	plug-in, developers can also report the corrected version of outdated code back
  	to the original Stack Overflow threads when they reuse outdated code and make
  	corrections to them.
    </div>
</div>

***
