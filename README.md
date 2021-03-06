Laptop
======

Laptop is a set of scripts to get your laptop set up as a development machine.

Mac OS X
--------

First, install [XCode](http://itunes.apple.com/us/app/xcode/id422352214?mt=12&ls=1). ($4.99, requires OS X 10.6.6 or higher)

Set up your SSH key if you haven't yet:

    ssh-keygen -t rsa

Then, run this one-liner:

    bash < <( curl -s https://github.com/thoughtbot/laptop/raw/master/mac )

Then:

    echo '[[ -s "/Users/`whoami`/.rvm/scripts/rvm" ]] && source "/Users/`whoami`/.rvm/scripts/rvm"' >> ~/.bash_profile
    source ~/.bash_profile

Install the latest version of Ruby and some useful gems:

    bash < <( curl -s https://github.com/thoughtbot/laptop/raw/master/ruby )

Ubuntu
------

First, install [Ubuntu](http://www.ubuntu.com/download).

Set up your SSH key if you haven't yet:

    ssh-keygen -t rsa

Then, run this one-liner:

    bash < <( curl -s https://github.com/thoughtbot/laptop/raw/master/ubuntu )

Follow the on-screen instructions to load RVM in your shell, and make sure you can run the rvm command.

Install the latest version of Ruby and some useful gems:

    bash < <( curl -s https://github.com/thoughtbot/laptop/raw/master/ruby )

Use gEdit for your text editor. You can [customize it with these instructions](http://blog.sudobits.com/2011/04/02/textmate-for-ubuntu-linux/).

What it sets up
---------------

* SSH public keys (for authenticating with services like Github and Heroku)
* Homebrew or apt-get (for managing operating system libraries)
* Git (for managing versions of code)
* Ack (for finding things in files)
* Postgres (for storing relational data)
* Redis (for storing key-value data)
* ImageMagick (for cropping and resizing images)
* RVM (for managing versions of the Ruby programming language)
* Ruby 1.9.2 stable (for writing general-purpose code)
* Bundler gem (for managing Ruby libraries)
* Rails gem (for writing web applications)
* Heroku gem (for interacting with the Heroku API)
* Taps gem (for pushing and pulling SQL databases between environments)
* SQLite and PG gems (for making Ruby talk to SQL databases)

It should take between 20-60 minutes for everything to install. (depends on your machine)
