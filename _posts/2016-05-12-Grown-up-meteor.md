---
title: Grown up Meteor
layout: post
category: gsoc
---

<p class="lead">
Meteor has recently released a new version of it's framework, Meteor is now at 1.3. It was at version 0.3 I guess, when the OGV project started.
The codebase on which OGV started, has grown up. That demands OGV to grow up.
</p>

From [meteor's official blog](http://info.meteor.com/blog/announcing-meteor-1.3):

> Today we’re excited to announce Meteor 1.3, the latest release of the Meteor JavaScript application platform. The focus of this major release is to help teams with production applications manage, scale, and test their Meteor codebases, and to continue our work to align the Meteor platform with the latest innovations in JavaScript.

Highlights of this update

* __Support for NPM packages:__ We can now use npm packages directly in Meteor app. These packages will run on both client and server if designed to do so by author. Thus we don't need to use wrapper packages from atmosphere, we can directly use npm package. To include a npm package, simple do `npm install` or `meteor npm install` if npm is not installed.
* __Built-in application testing:__ Meteor now includes ability to perform testing at application level. There are two testing modes, unit testing and integration testing. In unit testing, only test modules are loaded, this is done by `meteor test`. In integration testing, complete app is loaded along with test modules. This can be done with `meteor test --full-app`.
* __New Corodova implementation:__ A complete rewrite of Corodova layer comes with Meteor 1.3. This corodova layer makes building native android and ios app from meteor code. New code build robust android and ios application by handling faulty application code. 
