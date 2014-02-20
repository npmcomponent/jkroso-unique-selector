*This repository is a mirror of the [component](http://component.io) module [jkroso/unique-selector](http://github.com/jkroso/unique-selector). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/jkroso-unique-selector`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
unique-selector
===============

[![Build Status](https://travis-ci.org/ericclemmons/unique-selector.png)](https://travis-ci.org/ericclemmons/unique-selector)

Given a DOM node, return a unique CSS selector matching only that element.
This is particularly useful when tracking in custom variables in analytics:


    document.addEventListener('click', function(event) {
        var selector = unique(event.target);
	
        _gaq.push(['_trackEvent', 'Engagement', 'Click', selector]);
    }, false);


Installation
------------

    component install ericclemmons/unique-selector


Tests
-----

    $ npm install
    $ make
    $ open test/index.html


License
-------

MIT
