---
title: Installing Meteor on FreeBSD
layout: post
category: gsoc
---

<p class="lead">
Finally I have been succesful in installing meteor on a freeBSD system. Although I was not able to install it locally, my mentor provided me with a digital ocean droplet to carry on with deployment of OGV. Here's a quick tutorial on how to install meteor on freeBSD system.
</p>

<h3>Making freeBSD ready for meteor installation</h3>
<p>To make freeBSD ready to install, we need to install few pacakges. We can do so by:</p>
<code>sudo pkg install -y bash git gmake mongodb node npm python</code>

<h3>Clone the Meteor from it's repository</h3>
<p>Next get the meteor clone built to support FreeBSD system</p>
<code>git clone --depth 1 https://github.com/4commerce-technologies-AG/meteor</code>
<p>Mostly, on some systems, you are done with installation, it's that simple ;). Do the following to check if meteor is installed correctly:</p>
<code>$HOME/meteor/meteor --version</code>

<h3>Building manually [optional]</h3>
<p>However, on some systems, we need to build the meteor ourselves</p>
<p>Do the following to build</p>
<p><code>cd $HOME/meteor</code></p>
<p><code>scripts/build-node-for-dev-bundle.sh</code></p>
<p><code>scripts/generate-dev-bundle.sh</code></p>
<p>Now Check the installation by following</p>
<p><code>$HOME/meteor/meteor --version</code></p>

<h3>Try creating app</h3>
<p>Try to create a basic app using <code>$HOME/meteor/meteor appname</code></p>
