---
layout: essay
type: essay
title: Manoa The Gathering Release Notes
date: 2017-01-15
labels:
  - Meteor
---
<img src="../images/landing.png" class="ui image">
Here you will find the current status of the project. Expect written updates biweekly.
### Past unresolved issues from Fall 2016
Last year, there were various issues that could not be resolved in time. It was a team effort and now I am the only member that shall be contributing to this project to hopefully get it to a working state. My responsibilities last semester were the layout of the overall site and the user interface, not the battle system which is currently in ruins. Apart from the functional chat room and direct messaging, the current battle system is not in a presentable state.

## Release Updates

## January 16
I finished my issues earlier than my other teammates when it came to the final deadline at the end of the year. As a result, I am unfamiliar with the final code merge state of the project and have ran into many issues that were left unresolved due to no time left. Visually, everything seems okay, but with light use, things began to fall apart. I have been trying to familiarize myself with the changes that have been done by comparing commits done by my past teammates and the little documentation has made things much harder. I am still trying to salvage what I can, and have been considering reverting to the last merge to master done by me and starting over from there instead of trying to debug unfamiliar code. The main black box component that has been introduced since my last code contributions was the installation of several new Meteor packages known as CollectionFS. Through some research, I found that it was a way to serve dynamic image collections to unique users, but the implementation was very incomplete and has introduced a Bcrypt Issue that I still have not solved yet. I managed to resolve the animation issues of page transitions, but there are still overflow issues in the tutorial pages if all dropdowns are expanded. I plan to focus my efforts on getting a functional card playing system, with aesthetics and robustness of error handling being on the backburner for now.

### Project homepage
Check out the <a href="https://manoa-the-gathering.github.io/">project homepage</a> for more information.

### Project on Github for developers
<a href="https://github.com/manoa-the-gathering/manoa-the-gathering.github.io">The Github repository for interested developers.</a>
