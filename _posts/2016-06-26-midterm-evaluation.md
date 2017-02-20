---
title: Mid Term Evaluation
category: gsoc
---

<p class="lead">
So here I am half way through GSoC. I just can't believe, it's already been a month since I am working on this project. Time sure fly.
This month was mostly concentrated on front end and database stuff. I am yet to take a deep dive into improving the model viewing expereince of an OGV user.
</p>

<h3>Summary of my GSoC work</h3>
<p>I am really thankful to GSoC for keeping me busy during my summer holidays. If it wasn't for GSoC I may have died of boredom. :P :D </p>
<p>Regarding OGV, Here's the summary of what I have been doing till now. For details, check out my daily logs.</p>
<ul>
<li>Removing code which is deprecated. Re-writing that code with newer syntax.</li>
<li>Removing code written twice</li>
<li>Adding schema to each collection</li>
<li>Implementing a robust database in OGV</li>
<li>A consistent way of notifications, which is by using sAlert notification</li>
<li>Redesigining the sAlert notifications </li>
<li>Adding share functionality</li>
<li>Adding a notification panel, that shows notification everytime someone loves/comment/shares your model</li>
</ul>

<h3>My experience</h3>
<p>It's fun to exchange messages using IRC, interacting with developers talking about Github PRs.</p>
<p>I have felt the same way long before when I was working on Wt, a C++ web framework. So GSoC revived those memories for me.</p>
<p>Another fun thing I like in GSoC is keeping a log, writing everything down. I do like to write things. I confess, I may not be very punctual in writing log, but I am making sure to write things down, as soon as possible.</p>

<h3>Doubts till now</h3>
<p>I was seeing the code and workflow of OGV today, and here are few doubts I would like to ask:</p>
<ul>
<li>In collection named <code>OgvSettings</code>, there's an attribute named <code>settingSwitch</code>, it's set to true by default. Neither we alter that value anywhere in code, nor we do check it's value. So is this reserved for some future use, or it was used in past and we no longer needed it.</li>
<li>In user profile, we are using an attribute named <code>countModels</code>, it's a number that stores the number of models uploaded by user. But sometimes the model uploaded is not converted because of converter issue. The number is still incremented. Thus showing wrong count of models. I feel it's difficult to manage this count variable, instead what we can do is <code>ModelFiles.find({owner:user_id}).count()</code> This will give us the total number of models uploaded and converted successfully of a specific user. It seemed a right approach to me.</li>
<li>In my proposal I wrote Mid term evaluation a week late, but since mid term evaluation is now, Automatic thumbnail generation couldn't be done before mid term. It will be first thing to do after mid term evaluation. I hope it's OK with you.</li>
</ul>
