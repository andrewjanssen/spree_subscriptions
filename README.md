Spree Subscriptions
==================

This extension allows administrators to mark certain products as
'susbscribable'. Shoppers can subscribe to those products, causing them to be
re-shipped to the shopper at a chosen interval.

Features
=======

* Subscriptions are per-week. EG: every week, every 2 weeks, every 16 weeks. No daily or monthly subscriptions, sorry!
* Subscriptions paid up-front, then delivered as many times as possible with the amount paid.
* Entire orders (of subscribable products) can be subscribed, not just single products.
* Subscription payments that fail are retried up to 5 times by default.

Future Features
===============

* Subscriptions will be postpone-able until a set 'resume_on' date.

Installation
========

Add the gem to your Gemfile:

    gem 'spree_subscriptions', github: 'DynamoMTL/spree_subscriptions.git'
    bundle install

Run the generator and the included migrations:

    rails g spree_subscriptions:install

Testing
-------

Be sure to bundle your dependencies and then create a dummy test app for the specs to run against.

    $ bundle
    $ bundle exec rake test_app
    $ bundle exec rspec spec

Copyright (c) 2013 [Dynamo], released under the New BSD License
