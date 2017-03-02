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

## Past unresolved issues from Fall 2016
Last year, there were various issues that could not be resolved in time. It was a team effort and now I am the only member that shall be contributing to this project to hopefully get it to a working state. My responsibilities last semester were the layout of the overall site and the user interface, not the battle system which is currently in ruins. Apart from the functional chat room and direct messaging, the current battle system is not in a presentable state.

## Release Updates

## March 1
For this Milestone, I was not very productive in making progress on my Naya draw functions. I had looked into "foreign keys" to get an understanding of how to integrate relational databases, but ran into some problems during integration. I had trouble trying to get the right syntax for mongo sample aggregation and inserting objects with additonal fields. Improper usage led me to experience a "Range Error: Maximum call stack size exceeded."

### Changes
  * No functional commits at the moment
  
### Upcoming
  * Work on inserting cards into a player hand collection with an additional id field to build the relations.

## February 15

### Report
I have spent a lot of time working with the CollectionFS package in meteor to store the binary images of cards in a deck on the server and then have the client download a copy of it onto their system when they want to use it. After a meeting with a professor experienced in database management, I realized that I could get away with just modfiying the image src paths to display them. However with this approach, I am currently stuck on how to draw a random entry from the collection. I discovered that in Mongo 3.2, a new operator $sample was introduced, which could return a random entry from a collection. However, I would need to remove the card after to prevent it being possibly selected again. Removing it would then affect the main server database that is shared amongst users. My professor also talked to me about foreign keys, and maybe integrating that with my json objects to build a relational database using user ids which I am currently looking into..

### Changes
  * Got CollectionFS working. Client successfully downloaded the binary files from the server.
  - Left the CollectionFS code in a separate branch, for possible custom cards in the future.
  - Rebuilt Naya deck collection without the CollectionFS package.
  - Downloaded full 60 card deck into the system
  - Built a new card table layout, trashed the old one.
  - Installed "meteorhacks: aggregate package," in hopes to use MongoDB's $sample aggregation to select random cards
  
### Upcoming
  * Work on draw, shuffle, playing functions with the cards in the shared server collection
  * Copy mechanics over to Affinity deck.

## February 1

### Changes
  * Reverted back to project state before merge of battle system after trying to debug through commit history.
  - Decided to use mongodb combined ith gridfs instead of the Amazon S3 implementation
  - Removed S3 methods, replaced with mongo implementations
  - Using original card placeholders. Will use UH versions once system is working.
  - Implemented separate deck collections and a new field collection
  - Switched the mlab db back to my own account
  
### Upcoming
  * Learn how to upload images to gridFS collections
  * Finish the deck collection filling.
  * Come up with an algorithm to handle card insertions from the client into the general field collection published.
  * Modify deck collection functions from the S3 implementation.
  
### Features pushed back to future milestones
  * Fix matchmaking system
  * Define preset zones for the field collection to publish to, based on metadata from FS.file instance.
  * Assigning unique sessions, creating a new field collection for simulatneous games
  * Update card arts
  * Give users ability for unique decks

## January 16
I finished my issues earlier than my other teammates when it came to the final deadline at the end of the year. As a result, I am unfamiliar with the final code merge state of the project and have ran into many issues that were left unresolved due to no time left. Visually, everything seems okay, but with light use, things began to fall apart. I have been trying to familiarize myself with the changes that have been done by comparing commits done by my past teammates and the little documentation has made things much harder. I am still trying to salvage what I can, and have been considering reverting to the last merge to master done by me and starting over from there instead of trying to debug unfamiliar code. The main black box component that has been introduced since my last code contributions was the installation of several new Meteor packages known as CollectionFS. Through some research, I found that it was a way to serve dynamic image collections to unique users, but the implementation was very incomplete and has introduced a Bcrypt Issue that I still have not solved yet. I managed to resolve the animation issues of page transitions, but there are still overflow issues in the tutorial pages if all dropdowns are expanded. I plan to focus my efforts on getting a functional card playing system, with aesthetics and robustness of error handling being on the backburner for now.

### Project homepage
Check out the <a href="https://manoa-the-gathering.github.io/">project homepage</a> for more information.

### Project on Github for developers
<a href="https://github.com/manoa-the-gathering/manoa-the-gathering.github.io">The Github repository for interested developers.</a>
