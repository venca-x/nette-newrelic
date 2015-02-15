Nette Newrelic
===============

[![Build Status](https://travis-ci.org/venca-x/nette-newrelic.svg)](https://travis-ci.org/venca-x/nette-newrelic) 
[![Latest Stable Version](https://poser.pugx.org/venca-x/nette-newrelic/v/stable.svg)](https://packagist.org/packages/venca-x/nette-newrelic) 
[![Total Downloads](https://poser.pugx.org/venca-x/nette-newrelic/downloads.svg)](https://packagist.org/packages/venca-x/nette-newrelic) 
[![Latest Unstable Version](https://poser.pugx.org/venca-x/nette-newrelic/v/unstable.svg)](https://packagist.org/packages/venca-x/nette-newrelic) 
[![License](https://poser.pugx.org/venca-x/social-login/license.svg)](https://packagist.org/packages/venca-x/nette-newrelic)



Addon for better monitoring Nette framework

Installation
------------

Add the nete-newrelic to your dependencies (you need composer):

        composer require venca-x/nette-newrelic

Configuration
-------------

config.neon

    services:
        newRelicListener:
            class: Vencax\NewRelicProfilingListener
            tags: [kdyby.subscriber]
    
    extensions:
        events: Kdyby\Events\DI\EventsExtension

It's all :-) Now you see nice sections in Newrelic.  