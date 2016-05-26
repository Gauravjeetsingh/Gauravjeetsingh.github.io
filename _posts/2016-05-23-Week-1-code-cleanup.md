---
title: Week 1 (code cleanup)
---

<p class="lead">
In this week as per my plan, I'd be doing a bit of code cleanup. This involves managing github repository, removing redundant code, making sure all the variable names are consistent and so on.
</p>

<div class="accordion">
<h3> May 25th </h3>
<div>
<p>The first activity of this day was to send a mail to BRL-CAD mailing list about the confusion I had regarding repo access.</p>

<p>As my first milestone involves doing some cleanup work. I needed access to the BRL-CAD's OGV repository. There are numerous branches for now and a number of pull requests that are yet to be reviewed.</p>

<p>So at around 12:05 AM IST I sent a mail to BRL-CAD mailing list and slept.</p>

<p>I woke up and checked my inbox, I had a reply from sean. As per his reply, in order to get access, one needs to send compulsory two Pull Requests that are flawless improvements to the current code. It is a nice way to maintain a Github repo.</p>

<p>I have previously sent some pull requests so asked for their review, and in the meantime, I started looking for something to work on, so that I can send one more pull request to OGV repository.</p>

<p>In late evening, Inder suggested going with deployment first, and later working on code cleanup.</p>
</div>
<h3> May 24th </h3>
<div>
<p>Today I had to go to my college for some event. This reduced my work hours. 
I read some stuff online about Meteor and thought of their implementation in OGV. As I previously told in my post "Grown up Meteor", Meteor now comes with inbuilt support to npm packages. So we can now use threejs, without its wrapper package ishwerdas:threejs.</p>

<p>Also, I tried to understand the OGV backend, how the conversion is taking place. I can't say I completely understood the procedure, but yeah, now I know how the stuff works.</p>

<p>That's all folks !</p>
</div>

<h3> May 23rd </h3>
<div>
<p>God blessed with an amazing weather to commence this coding period. Such a relief from scorching days. Also, today I finished with my university exams and thus ready to code. This week's milestone is to clean the existing code. To finish what's already started seems a right approach. </p>
<p>After this cleanup, my next milestone is to successfully deploy the cleaned version of OGV.</p>
<p>Regarding work, I reviewed basic code, fetched all the branhes on my local machine, and started analysing what's in each branch, the suggested branch to work upon is gsoc2015-merged. I am trying to find if there's any line of code we need from some other branch. I am thinking to create github branch structure somewhat similar to given below:
<ul>
<li> Master (containing stable code)</li>
<li> Released (containing code of latest release)</li>
<li> dev (containing unstable under development code) </li>
</ul>
</p>
</div>

</div>
