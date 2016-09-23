---
layout: essay
type: essay
title: IDE's.. Why?!
date: 2016-09-22
labels:
  - IntelliJ
  - Coding Standards
---
## Code NOW or later
Integrated Development Environments. Why go through the trouble of setting one up and learning all the menu options
when you can just code instantly in JSFiddle?! I always used the built in vim that comes with the command shell to code all
my C/C++ programs. When I started diving into Javascript development, I was relieved that JSFiddle existed. You can do 
whatever you want in these editors. Sets up in a second or two, letting you focus on the real coding problem at hand.

Now with IDE's, its always the same process: Open. ... Do you want to start a new project? Yes. What kind of project? ...
Okay what would you like to name it? ... Where should it be saved? ... Now here is your codespace. Oh wait, you need to
make a file. What do you want to call it? !!!
<hr>
## Okay, but what if you need multiple files? Open 20 JSFiddle/Vim windows?

For complex projects, then IDE's are definitely better yes. I remember having to make multiple shell windows and sizing all of them so I could fit them in my screen. Or vim-ming in and out of files. In terms of starting out though, I feel that using a bare editor and a compiler improves your skills in debugging programs.  It improves your ability to catch erroneous code yourself while coding instead of having an IDE highlight where all your errors are. Only when one is proficient in the language, can I then see the need for IDE's. You already know what you want and code completion can be very helpful. Beginners may just abuse code templates and not even feel the need to remember everything. Type a few lettters, press ctrl-space and bam! Instantly there. Don't even need to look at what was put in, its guaranteed to be correct. 
<div class="ui fluid image">
<div class="ui red right ribbon label">Code Completion is Awesome!</div>
<img src ="/images/ccomp.png">
</div>

### Coding Standards
But! Now you tell me we have to code a certain way? That's more work though! Yeah it is. Adding that extra space every time soon adds up and increases your final coding time by a minute or so, but still! Definitely more work. But then I soon realized that most of my complaints seemed only logical since the only person that will be reading my code is myself. It feels more comfortable reading code in the way I like seeing it. However in engineering, work is usually accomplished by teams. We all code differently to some extent. Some prefer string concatenation, others like template literals. Single quotes vs double quotes. Using arrow functions over the "real" function definition. 
<div class="ui fluid image">
<div class="ui orange right ribbon label">Too many blank lines?! <br> [1, 2, 3, 4] is the same thing!</div>
<img src ="/images/eslint.png">
</div>
In scenarios like these though, whether one likes it or not, I do believe that adhering to a general coding standard is very helpful. ESLint seems a little too strict on some things in my own honest opinion. 
<hr>
## Verdict so far?
Using coding standards in the sense to improve readability is good to *some* extent. Using coding standards that directly
affect the code though, like using const or let instead of var, is great. For these things, the coding standards built into
the IDE definitely can help one learn the "proper" way to do things. Bare editors don't even bother with things like this,
and assume the one coding knows how to code appropriately. For self-interests, doing whatever is totally fine. But once more
people begin to get involved with the same code/project, a coding standard is a must to prevent internal code from becoming
way more confusing than it needs to be. But if a team consists of master software engineers that are total geniuses, then in
cases like that, coding standards would probably slow them down. They should be allowed to code however they want, confident
that the other members on their team can decipher their code easily. Or they 

