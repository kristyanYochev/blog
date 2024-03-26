+++
title = 'Taking Off'
date = 2024-03-26
+++

I have been dreaming to make and publish a game practically since starting to
learn programming when I was 13. I have dabbled a bit with different engines and
game programming frameworks, but I haven't really made anything beyond copying
popular games for the sake of learning how they are made. Now having studied
Systems Programming in high school and on the verge of finishing my bachelor's
degree in Computer Science, I feel it's about time I try and do it for real.

I want to make a game about managing and expanding an airport, taking it slowly
from a simple airstrip to the likes of London Heathrow, Amsterdam Schiphol, and
Paris Charles de Gaulle, with the twist that they're going to have to direct
that traffic by themselves, at least in the beginning.

## Inspiration

My main inspiration for this game are other games, which I will discuss in a
bit. I will be pointing out the bits I like and don't like about which one and
discuss what I can add from that game into mine, keeping in mind that all these
features and mechanics will need to be prototyped and tested to validate them.

### Rail Route

While I play quite a few games, one that I've been playing regularly since it
was in early access is [Rail Route](https://railroute.eu/). The combination of
dispatching and tycoon-like gameplay is so good, I think it has potential
outside the tracks. The premise behind Rail Route is quite simple - you dispatch
trains, which earns you money and experience points. You can spend the money to
expand your network and the experience points on various upgrades such as
automatic signals, faster tracks, and a number of sensors allowing for automated
routing.

Rail Route does a ton of things right: the balance of the game is good, the
three game modes are so good they can be games unto themselves, the custom map
editor has led to a community of rail enthusiasts making maps of their favourite
regions alongside fictional layouts, the interface is easy to understand and the
tutorial is fantastic.

It all comes down to the attention to detail the developers have had from the
very beginning. Each mechanic they've added was well explained and fits well
with the rest of game, contributing to the coherency of the game.

### OpenScope

I have tried out a bunch of different ATC simulator games, and while some are
better than others, none of them quite hit the mark for me. The closest one I've
found so far is [OpenScope](https://www.openscope.co/). It has a beautiful UI,
strikes a good balance between realism and fun, and is overall a nice game on
its own.

On the balance between realism and fun, it is more on the realistic side than
what I'm looking for. This is not inherently bad, but as I want my game to be
appealing to a wider audience, it probably isn't a good idea to make them read
airport charts.

Speaking of not being understandable by the general audience, the in-game
tutorial is just a bunch of small text messages, which caused me to just skim
over it the first time I played it. After properly reading through it and
getting comfortable vectoring aircraft around, I wanted to try out the more
advanced stuff like RNAV routing, SIDs, and STARs. This led me to the builtin
airport guides, which vary in their information content from airport to airport.
For some airports, the guide has the procedures laid out in some form, while for
others its nothing more than a link to the navigational charts for it.

## The Game is in The Details

Given that the basic premise of my game is a fusion of ATC simulator and tycoon,
it is vital to consider which features will work together and which ones to
throw out. The only way to know for certain is to build a prototype and test it
with real players, but I still need to figure out what I need to put in the
prototype. In order to do that, I have to set some criteria:

1. The prototype needs to be as small as possible. If a feature is not strictly
   needed, it doesn't get added in.
2. The prototype must incorporate the core of the gameplay experience I aim to
   deliver. E.g. air traffic controlling and basic building mechanics must be
   present.
3. The prototype need not look fancy. My art skills are poor, so the prototype
   is going to consist of mostly programmer art. If I can easily find an asset
   online, I will use it.

### At The Heart of It

Given criteria 1 and 2 from above, I have to ask myself what the core gameplay
should be. I will look at the major game components and distill them to the
smallest possible size while preserving their identity.

For the tycoon side of it, that means having just one currency (so no XP and the
likes), a minimal set of elements to build, and a basic accept/reject for
incoming flight plans. In terms of the building elements, every airport has at
least one terminal building, runway, taxiway, and some place for planes to park
(known in aviation as a 'stand').

On the ATC side, that means some sort of interface to clear aircraft for takeoff
and landing, give them directions and altitudes (called 'vectoring' in the
industry), and tell them which taxiways to use when on the ground.

### Teaching the Game

Air traffic control is a complex task and if I want to incorporate it into the
game, I will need to find a way to make it more approachable to the average
person. Part of that would be just the way information is presented, visually
drawing aircraft's paths and player-defined routes, so they can see exactly
where planes will go.

While the information presentation definitely helps, making the game tutorial
more hands-on would have an even bigger impact on learning. Rail Route's
tutorial is a fantastic example of the style of tutorial I'm aiming for. This
kind of learning is called _kinesthetic learning_, and possibly the best summary
of that is the
[video on complex games' tutorials by Game Maker's Toolkit](https://www.youtube.com/watch?v=-GV814cWiAw).

### The Boring Stuff

Seeing as I'm in my last months of studying, I will be primarily focusing on
finishing my degree, so the prototype is not going to see the light of day for
quite a while. The year is slowly coming to a close, so my workload is not
immense, but I still won't be able to work full-time on the prototype until
mid-July. Still, it is small enough that by then it should be in a mostly done
state, even with my current schedule.

In terms of engine, I'm going with Godot, mostly because of its nice UI system
and its support for C# as a scripting language.

## Big Picture

This is just the start of this game development journey, I have no idea how long
it's going to take or whether it will ever finish. I hope it gets to see the
light of day and be enjoyed by many people. See you in the next one!
