Talk UI Router
==============

For the ngParis meetup of the July the 24th, 2013, I'll be presenting UI Router. This GitHub aims to contains demo and slides.

[AngularJS: We must go deeper](http:// www.meetup.com/AngularJS-Paris/events/126735742/)

Demo
----

For the demo, I choose to clone the very good code from [Year Of Moo](http://www.yearofmoo.com/) second article on Angular's animations.

This code base is great for animations but routing can be improved. I demonstrate this by including AngularJS UI Router to handle states while keeping animations working.

As I intend to work with as up to date as possible versions of libraries, you need to build AngularJS and UI Router which I installed in bower with their real GitHub repository.

        npm install
        bower install
        cd app/bower_components/angular.js
        grunt
        cd ../ui-router
        grunt

Modifications which as been made :

* Merge code with fresh 0.3.0 ``yo angular`` code base
* Replace ?q=search by ui router state #/q/{search}
* Replace appFocus directive by nested route /focus/{id} wiring same animations with ui-view and ng-show

Feature lost (at that point) : opening of the focus on the same line as the thumbnail.

Slides
------

Slides are made with [RevealJS](https://github.com/hakimel/reveal.js)

I wrote the slides in english even if the talk will be in french