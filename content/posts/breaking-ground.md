+++
title = 'Breaking Ground'
date = 2024-03-26
draft = true
+++

I have been dreaming to make and publish a game practically since starting to
learn programming when I was 13. I have dabbled a bit with different engines and
game programming frameworks, but I haven't really made anything beyond copying
popular games for the sake of learning how they are made. Now having studied
Systems Programming in high school and on the verge of finishing my bachelor's
degree in Computer Science, I feel it's about time I try and do it for real.

## The Game

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

Since my game wants to incorporate air traffic control as a game mechanic, I
will need to find a way to make that task more approachable to the average
person. Part of that would be just the way information is presented, visually
drawing the instrument procedures onto the map as routes seems like a better way
to present them than linking to a PDF. This also going to be helped in no small
part by the fact that player is the one who's making these procedures.

While the information presentation definitely helps, making the game tutorial
more hands-on would have an even bigger impact on learning. Rail Route's
tutorial is a fantastic example of the style of tutorial I'm aiming for. This
kind of learning is called _kinesthetic learning_, and possibly the best summary
of that is the
[video on complex games' tutorials by Game Maker's Toolkit](https://www.youtube.com/watch?v=-GV814cWiAw).

Another thing I want to incorporate into my game is ground control, rather than
taking OpenScope's approach of planes magically appearing at the beginning of
the runway before clearing them for takeoff and magically disappearing right
after landing.
