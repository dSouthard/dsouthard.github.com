---
layout: post
title:  "Setup Instructions"
date:   2015-12-06 14:36:23
---

<span class="image featured"><img src="/images/setup.png" alt=""></span>

Initial Setup Requirements
---------------------

The latest version of Jekyll is 3.0.1, released 11/17/2015. This is the version we will be working with for this presentation. The following requirements are necessary before you can set up your first Jekyll website:

* Ruby (v2 or above for Jekyll 3)
* RubyGems
* Linux, Unix, or Mac OS X (I'll be assuming you're on Ubuntu 14.04)

All in all, you can be setup in less than 30 minutes, provided nothing goes wrong!

#### Note:

You can either switch to your sudo account or add the sudo keyword in front of the following terminal commands.

Installing Ruby/RubyGems
---------------------

Unfortunately, the default package of Ruby installed when using the system's package manager does not install the latest version of Ruby. It installs a version which is incompatible with the latest version of Jekyll (version <i>1.9.3p484</i>, to be specific). A slightly more involved installation is required, as described in the following:
<br>

#### Step One
The first step is to install some dependencies for Ruby.
<p>
    >> sudo apt-get update <br>
    >> sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev
libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev
libcurl4-openssl-dev python-software-properties libffi-dev
</p>

#### Step Two
There are several different methods of then installing Ruby, but the recommeded method is by using rbenv: 
<p>
    >> cd<br>
    >> git clone git://github.com/sstephenson/rbenv.git .rbenv<br>
    >> echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc<br>
    >> echo 'eval "$(rbenv init -)"' >> ~/.bashrc<br>
    >> exec $SHELL<br>

    >> git clone git://github.com/sstephenson/ruby-build.git ~/.rbenv/plugins/ruby-build<br>
    >> echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc<br>
    >> exec $SHELL<br>

    >> git clone https://github.com/sstephenson/rbenv-gem-rehash.git ~/.rbenv/plugins/rbenv-gem-rehash<br>

    >> rbenv install 2.2.3<br>
    >> rbenv global 2.2.3<br>
</p>

At this point, you should have Ruby running on your machine! Just to check, try:
<p>
    >> ruby -v
</p>
You should get `ruby 2.2.3p173`. If not, you will need to try the setup again, perhaps with <a href = "https://gorails.com/setup/ubuntu/14.04#ruby-rvm">another method.</a>


Installing Jekyll with RubyGems
---------------------

The easiest and best way to install Jekyll at this point is by using RubyGems :
<p>
    >> gem install jekyll<br>
</p>

You are now ready to go!

