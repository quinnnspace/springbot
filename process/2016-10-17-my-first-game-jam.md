---
layout: post
title: On mental health, my first game jam, and finishing things
---
So here's the thing: life isn't really going well for me right now. I'm not interested really in throwing a pity party for myself, but I think it's important to be candid here, even if it doesn't paint me in the best light. First and foremost, I'm writing this for myself, and I'm also trying to make games for myself primarily, but that's getting ahead of things.

## Mental struggles

After struggling with anxiety and depression for most of my adult life, and trying various different strategies to overcome these problems, things became much worse 2 years ago, when I stopped being able to work, along with being unable to do most of the other things that made up my day to day life. Since then, while, in different ways and at different times, things may have improved or gotten worse, overall I feel I've become entirely stuck in this state of helplessness. Even things like showering, cooking, cleaning and all the other things we do to take care of ourselves, became insurmountable.

In particular, programming, which is one of the talents that has defined me throughout my life, has become almost impossible. Lack of motivation, ability to concentrate and, honestly, pervasive despair and dread all combine to create a difficulty that I could not have imagined a few years ago. It's incredibly disheartening.

Making games: that's something that has always held a significant allure, both in the superficial sense of the idea of 'who I wanted to be seen as' and in the deeper sense of the complex frustrations involved in doing it day to day. I loved the idea of being a solo, experimental artist with complete control over, and responsibility for, my creations; solving weird problems and creating things and, maybe, understanding myself and the universe a little bit more each time. Naturally, any time I tried to persue this vision, I smacked straight into my own limitations and the discomfort of doing difficult things. Being reasonably intelligent, avoiding discomfort is something I've become quite masterful at; dealing with discomfort when it is unavoidable or worth facing: not at all.

That's mostly enough, most of the time, when mere survival is the goal. That doesn't work for me anymore.

## The Pippin Barr 'GAME IDEA' Game Jam

So, enter [Pippin Barr](http://www.pippinbarr.com/about/ "About Pippin Barr"), a game designer (among other things) who posts a large number of intriguing game ideas from his [Twitter account](https://twitter.com/pippinbarr/ "Pippin's twitter page"), and [Conor Mccann](http://theworkhouse.co/ "Conor's Portfolio"), who decided that it was about time some of these ideas got turned into actual games and created [The Pippin Barr 'GAME IDEA' Game Jam](https://itch.io/jam/the-pippin-barr-game-idea-game-jam "Game Jam page on itch.io").

Now, I've been drawn to game jams for quite some time now, even attempting to begin a few from time to time, but this is the first time I've gotten anywhere with them. I heard about this one a month-or-so ago, and I thought that this jam was exactly the right one for me, but it was only once a few work-in-progress screenshots started appearing last week that I realised it had actually started and if I wanted to grab this opportunity, it was now or never. I looked through the [list of ideas](http://theworkhouse.co/transfer/game_ideas/ "A very long list of game ideas") and saw a few that seemed achievable in the small amount of time before submissions were due.

### Actually making a thing

I mentioned above how even everyday chores had become insurmountable. This is not hyperbole: doing anything these days is far more difficult than they have any right to be, and even if I manage to complete a task, it takes almost everything I have, and leaves me exhausted and unable to cope. It sucks, frankly. But then again, I sitting here writing about how I finished a game jam, so things may be slowly improving.

Saying that, it was important to choose a simple idea, and the one I decided on was perfect in it's limitations:

    ░ GAME IDEA
    ░░ 
    ░ JUMPING 
    ░░ 
    ░ BUT IT'S ONLY 
    ░ JUMPING 
    ░ FOR JOY 
    ░░ 
    ░ YOU DON'T GET TO 
    ░░ GO ANYWHERE 
    ░░░ OR SEE ANYTHING 
    ░░░░ OR KILL ANYONE 

Here was an idea that I could return to any time my mind started to overcomplicate things, and keep me from being overwhelmed.

While I'm keen to learn to work with `<canvas>` tags and the other basics of HTML5 game development directly so I have a good grasp of the fundamentals, it was most important for me, this time, to get something on screen and working. Earlier this year I managed to dedicate a month to learning javascript more fully than I have before so after a quick web search and reading a few tutorials I found [phaser.io](http://phaser.io), a handy framework to help take care of all the annoying things, like compatibilty and such, while letting me actually write the code to make things work. 

Frameworks are all well and good, but without any assets to work with, my options would be fairly limited. Text and geometric shapes can sometimes be enough, but not this time. So I had to learn, quickly, how to draw myself a main character: someone to jump, joyously if possible. I've never been a particularly gifted artist, but, in the grand tradition of game jams, I gave myself permission to suck.

### I suck at pixel art, but that's OK

With half-remembered tips from pixel art tutorials read years ago bouncing around my head I jumped on to [Piskel](http://www.piskelapp.com Simple but powerful pixel art editor and animator) and got to work. And then stopped, brain quickly fried and dripping out my ears.

![A badly drawn, retro-styled robot]({{ site.url }}/assets/20161017/00001.gif "Pixel Art Attempt Number 1")

And in another reality, that was that. Somehow, not this one though. After coming back and working on my first attempt some more, with regular breaks to pace around my house shaking and, at times, in tears, I started work on a second draft of my jumping character, this time with some simple animation.

![Another badly drawn, retro-styled robot]({{ site.url }}/assets/20161017/00002.gif "Pixel Art Attempt Number 2")

Simple though this was, it was really grinding down my mental resiliance. 'Am I too unwell for this stuff?' Doubts and frustrations abounded, but I carried on, taking any short bursts of productivity I could find over the course of several days to refine it. I was aware that if I didn't hurry I wouldn't have any time left to program anything, but I also felt that getting the animation and art to a state that I was happy with was the key to this project. Besides, while working away at the art, the shape of the game as a whole was forming in my head. Eventually, 'springbot' was born, and I'm ridiculously proud of it:

![A spritesheet of 'springbot' animation]({{ site.url}}/assets/20161017/spritesheet.png "Spritesheet of 'springbot'")
![A less badly drawn, retro-styled robot]({{site.url}}/assets/20161017/00003.gif "Final animated version of 'springbot'")

### Deadline approaching: making things interactive

With just a spritesheet, a few rapidly generated sound effects from [Bfxr](www.bfxr.net "Bfxr sound effects generator"), and the model that'd been forming in my head of how things would work, it was time to code it up. Time was against me: I only had a few hours before the submission deadline, and in many ways I was fighting against myself. Still, with the momentum I'd gained, I was excited by the possibility that I might get things done.

Fortunately, using a framework made things a lot easier, though I had to quickly learn how to make it do what I wanted. With documentation and examples on one screen and text editor on the other, I started typing. Here, I was in my element. This was where I could make a tiny amount of magic happen. With the limits of the original idea, along with only a small amount of time to work with, I was able to create something very simple: more a toy than any real kind of game.

But I had fun playing around with the simple mechanic: solving problems and making it feel right.

And I finished. And that is something I haven't done with anything in a long time.

<iframe frameborder="0" src="https://itch.io/embed/91801?bg_color=ffffff&amp;fg_color=ebebeb&amp;link_color=603286&amp;border_color=4b4156" width="208" height="167"></iframe>

## Reflections on finishing things, and the value of the journey

I'm being careful not to paint this as some huge victory. But it is a first step.

The toy itself will not really be of interest to most people: it's very basic and doesn't really have enough to do. It is a curio more than anything else. But in the process of making it I found out a lot: about programming, about games, and mostly about myself. It was a real challenge: one I was able to overcome. It took a great deal out of me, and I'm not sure I'm going to be able to parley this into anything else yet. I've learned, in the past, the very real dangers of pushing myself too far, and things are very delicate right now: I don't want to make that mistake again. It terrifies me.

But I made a thing. And that isn't nothing.