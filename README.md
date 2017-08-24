Nette Newrelic
===============

[![Build Status](https://travis-ci.org/venca-x/nette-newrelic.svg?branch=v1.0)](https://travis-ci.org/venca-x/nette-newrelic) 
[![Latest Stable Version](https://poser.pugx.org/venca-x/nette-newrelic/v/stable.svg)](https://packagist.org/packages/venca-x/nette-newrelic) 
[![Total Downloads](https://poser.pugx.org/venca-x/nette-newrelic/downloads.svg)](https://packagist.org/packages/venca-x/nette-newrelic) 
[![Latest Unstable Version](https://poser.pugx.org/venca-x/nette-newrelic/v/unstable.svg)](https://packagist.org/packages/venca-x/nette-newrelic) 
[![License](https://poser.pugx.org/venca-x/nette-newrelic/license.svg)](https://packagist.org/packages/venca-x/nette-newrelic)

Addon for better monitoring Nette framework

Branch v 1.0.x is for Nette 2.4
------------

Installation
------------

Add the nete-newrelic to your dependencies (you need composer):

        composer require venca-x/nette-newrelic @dev

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
