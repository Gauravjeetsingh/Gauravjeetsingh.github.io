---
title: Dockerizing LibreHatti
layout: post
category: default
---

<p class="lead">
LibreHatti is an open source CRM solution built in Django. This post tells how to run LibreHatti in a docker container.</p>
<p>Docker is an application that makes it simple and easy to run application processes in a container, which are like virtual machines, only more portable, more resource-friendly, and more dependent on the host operating system. <a target='_blank' href='https://www.digitalocean.com/community/tutorials/the-docker-ecosystem-an-introduction-to-common-components'>Read More about dockers</a></p>


<div class="accordion">
<h3>Install Docker</h3>
<div>
<p>Follow <a target='_blank' href="https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-16-04">this</a> guide to install the latest version of Docker.</p>
</div>

<h3>Clone LibreHatti </h3>
<div>
<p>Clone Librehatti from my forked version. This forked version have been configured to be ready to use from a docker container.<br>
<code>git clone https://github.com/gauravjeetsingh/librehatti</code></p>
</div>

<h3>Add MySQL password to config file</h3>
<div>
<p>After cloning, you will see a file named <code>docker-compose.yml</code>.</p>
<p>Open that file and add your root password of mysql server installed locally on your machine. See the line no 13 of this file.<br>
<code>	  - MYSQL_ROOT_PASSWORD=YOUR_MYSQL_ROOT_PASSWORD</code></p>
</div>

<h3>Build docker image </h3>
<div>
<p>Everything's ready, it's time to build this docker image<br>
<code>docker-compose build</code></p>
</div>

<h3>Add tables in the database</h3>
<div>
<p>To add tables in database as per your app, you can run the syncdb app of python in docker container as following<br>
<code>docker-compose web run python src/manage.py syncdb</code></p>
</div>

<h3>Run the app from docker container</h3>
<div>
<p>To run the app, simply run <code>docker-compose up</code></p>
<p>Open your browser at <code>http://0.0.0.0:8000</code></p>
</div>
</div>

