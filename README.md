Overview
========

This is a simple Symfony bash completion script designed to work with Symfony 1.4.

Inspiration and some code have been borrowed from:

* https://github.com/biko2/symfony_complete
* http://trac.symfony-project.org/wiki/BashCompletion

Features
========

* namespace completion
* task completion
* option completion
* option value completion for some well known options, such as
    * --env - completes against 4 hardcoded environments: prod, dev, qa, test
    * --application - completes against the dirs found in <sf_root>/apps
    * --connection - completes against configured connections in databases.yml
* caches task and option/argument lists and refreshes it once a week

Installation
============

Copy etc/bash_completion.d/symfony to the appropriate location in your system.
Depending on your distribution, this could be /etc/bash_completion.d/ for global availability or ~/.bash_completion.d/ if you only want to enable it for your user.
