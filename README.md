Heroku buildpack: Perl
======================

This is a Heroku buildpack for Okinawapm SlackBot.

Usage
-----

Example usage:

    $ pwd
    /Users/CodeHex/.ghq/github.com/OkinawaPM/SlackBot

    $ heroku create --stack cedar --buildpack https://github.com/OkinawaPM/heroku-buildpack-perl.git

    $ git push heroku master
    ...
    -----> Heroku receiving push
    -----> Fetching custom buildpack
    -----> Installing dependencies

Libraries
---------

Dependencies can be declared using `cpanfile` (recommended) or more traditional `Makefile.PL`, `Build.PL` and `META.json` (whichever you can install with `cpanm --installdeps`), and the buildpack will install these dependencies using [cpanm](http://cpanmin.us) into `./local` directory.

