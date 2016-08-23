---
title: Final Evaluation
---

<p class="lead">
Like all good things, GSoC also had an end date. In this post I will try to summarise what I did in 13 week GSoC time period.
<table>
<tr>
<td><a target="_blank" href="http://138.68.52.118:3000/">Live Demo</a></td>
</tr>
<tr>
<td><a target="_blank" href="/commits">My Github Commits during GSoC period</a></td>
</tr>
<tr>
<td><a target="_blank" href="/pullrequests">Pull Requests I made</a></td>
</tr>
<tr>
<td><a target="_blank" href="/status">Brief status report</a></td>
</tr>
</table>
</p>

<blockquote>
<b>✌ Good News</b>
<p>I asked my university professor, and she agreed on continuing OGV as my university project. So I shall continue the same pace of development atleast till December.</p>
</blockquote>

<h3>Major changes that are live on OGV</h3>
<ul>
<li><b>Robust Database: </b> A valid and tested schema is added to the collections <code>OGVSettings, Meteor.user, Comments, Lovers, Posts, Notifications, SharedModels</code></li>
<li><b>Deployment: </b> Currently OGV is running on a freeBSD system, which was a major requirement to get OGV to production. However a more robust automated deploy that includes automatic fetching from github, and assigning a domain name to meteor service is still in TODO list. <a href="http://138.68.52.118:3000/">Go to live verison</a></li>
<li><b>Notifications: </b>A complete redesign of sAlert notifications. Also added a notification panel, providing with notification of activity on user's uploaded model.</li>
<img src="/images/notification.gif">
<li><b>Sharing Models: </b>Now user's can share the model apart from loving or commenting on them</li>
<li><b>Redesign Search: </b>A complete UI brushup of search in OGV.</li>
<img src="/images/search.gif">
<li><b>Thumbnail Generation: </b>Instead of uploading a image for a preview in news feed, we can now take snapshot of rendered view of model as a preview image</li>
<li><b>Model viewer tools: </b>Now you get a set of tools in model viewer. These tools enable user to show/hide parts of the uploaded model. Also there is a option to assign a different color to each part of model. Thus one can easily distinguish between different parts a model have.</li>
<img src="/images/modelviewer.gif">
<li><b>Progress bar: </b>Added a progress bar that shows the live conversion percentage of converting a g file to number of obj files.</li>
<img src="/images/conversion.gif">
<li><b>Public/private models: </b>A user can now choose the viewer audience between public, only me and followers only</li>
<li><b>UI/UX Improvements: </b>There have been a lot of UI/UX improvements in OGV. One of them is of the header navigation bar. Too much icons confused the user what each icon does. Also on smaller screens it seemed total messed up.</li>
<img src="/images/menu.gif">
</ul>

<h3>Merging Obj files</h3>
It was this one task that I couldn't complete in GSoC period, but it sure would be done in some time. I have spent significant amount of gsoc time period in this. I need to find a logic, a way to reduce the number of obj files that are generated for each g file. This will bring no change to user view, but will speed up the things real fast.
