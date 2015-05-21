OUT OF ORDER
=========
this is not operative... yet...

dtIMB.DEVcrew
=======

[![Build Status](https://travis-ci.org/aleph1888/ng-elgg.png?branch=master)](https://travis-ci.org/aleph1888/dtimb.DEVcrew_DECK)

A secure, offline-capable, mobile-first web client for [Elgg](http://elgg.org) built with AngularJS.

Demo
----

http://aleph1888.github.io/dtimb.DEVcrew_DECK/

Installation
------

```sh
npm install -g volo grunt-cli
git clone https://github.com/aleph1888/dtimb.DEVcrew_DECK
cd dtimb.DEVcrew_DECK
npm install
volo update
grunt
```

Note also https://github.com/aleph1888/dtimb.DEVcrew_DECK/issues/1

This will set you up with a local version of the UI.


Browser Support
-----
Latest 2 versions of modern browsers.

Initial development is only happening on Chrome (desktop and mobile).
This is to give me freedom to experiment with the cutting edge of web tech.
As ng-elgg stabilizes and people start using it more seriously,
more effort will go into cross-browser support.

Modern browsers auto-update, so the long term plan is to only support
the latest browser versions, including for mobile browsers.

Any cross-browser support efforts should be largely transparent to
this project and the developers utilizing this project. We want to
avoid any kind of feature detection or UA detection in the project code itself.
It's best if that code goes into elgg-grunt so that it is just an
invisible part of the build process.

Why dtimb.DEVcrew_DECK?
------
Because http://ismy.band platform needs a deck to manage band-groups...

### Deck (dtIMB.DEVcrew)
It is adeck for group-band Client rendered UI    for    http://ismy.band as REST/RPC Api WEBSERVICES platform.
    
### Bands
To join-in, as we call it: band-joining, you just need a band-name and a band-domain...
i.e.: Meet "La Banda de Aranda", http://tic.ninja band from l'H...
http://dtimb.ismy.band/devcrew/blog/view/237/is-my-band-portada-seccion-join-in

### So, a band is...?
What is? / ¿Qué es? IS MY BAND How does it works? / ¿Cómo funciona? en el grupo Is My Band (TIC Ninja) 
http://dtimb.ismy.band/devcrew/pages/view/236/what-is-%C2%BFque-es-is-my-band-how-does-it-works-%C2%BFcomo-funciona    




FORKING:

ng-elgg
=======

[![Build Status](https://travis-ci.org/ewinslow/ng-elgg.png?branch=master)](https://travis-ci.org/ewinslow/ng-elgg)

A secure, offline-capable, mobile-first web client for [Elgg](http://elgg.org) built with AngularJS.

Demo
----

http://ewinslow.github.io/ng-elgg/

Installation
------

```sh
npm install -g volo grunt-cli
git clone https://github.com/ewinslow/ng-elgg
cd ng-elgg
npm install
volo update
grunt
```

Note also https://github.com/ewinslow/ng-elgg/issues/1

This will set you up with a local version of the UI.


Browser Support
-----
Latest 2 versions of modern browsers.

Initial development is only happening on Chrome (desktop and mobile).
This is to give me freedom to experiment with the cutting edge of web tech.
As ng-elgg stabilizes and people start using it more seriously,
more effort will go into cross-browser support.

Modern browsers auto-update, so the long term plan is to only support
the latest browser versions, including for mobile browsers.

Any cross-browser support efforts should be largely transparent to
this project and the developers utilizing this project. We want to
avoid any kind of feature detection or UA detection in the project code itself.
It's best if that code goes into elgg-grunt so that it is just an
invisible part of the build process.


Why ng-elgg?
------

### No more XSS
tl;dr: We accomplish this via a strict Content-Security-Policy and Angular's
automatically contextually escaped templates.

ng-elgg is based on AngularJS. Angular templates sport what is called 
"automatic contextual escaping" which means that all the right escaping rules
are applied automatically to template variables on output, without developers
needing to remember to be diligent about escaping user input in the right way
and in the right order every time. This is notoriously difficult to do and
basically impossible to do perfectly on a sufficiently large codebase, so
automatic escaping works wonders.

For times when you do want to display user-generated HTML, Angular provides a
client-side HTML filter that is very effective at beating XSS attacks.

Finally, ng-elgg ships with the strictest possible Content-Security-Policy 
turned on by default. For modern browsers with support for CSP, this makes
XSS next to impossible, since even if Angular's filters were somehow beaten,
the browser would simply ignore the resulting inline or untrusted, external scripts.

I am confident that these technologies put XSS attacks behind us for good,
yet very few frameworks that I'm familiar with have taken a hard stance on this,
most likely because doing so would break existing app functionality. ng-elgg
comes with no baggage of legacy, so we're free to do this correctly from
the start.


### Metrics
The best way to get insight into your users' experience using your app is to
measure everything.

ng-elgg comes out-of-the-box integrated with Google Analytics. But we go way
beyond just tracking pageviews:

 * Abandonment rates for every form (TODO)
 * Which parts of the UI are users interacting with (TODO)
 * How long is the transition from page to page (Done!)
 * All the exceptions you're getting and how many (TODO)
 * A/B experiments framework built in (TODO)

Each of these can give you really good insights into where your app needs
improvement and will help you focus on the low-hanging fruit first.


