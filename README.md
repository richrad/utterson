# Mister Hyde

Mister Hyde is your friendly web editor build for [Jekyll][jekyll] sites. It is in a **very early state** at this point, please read about the features and the roadmap further down in this document.

## Get started

It's fairly simple to get started and test Mister Hyde:

    git clone git@github.com:mister-hyde/mister-hyde.git
    cd mister-hyde
    bundle install
    rackup

Visit http://127.0.0.1:9292/ in your browser and you should see an empty list of Jekyll sites. Either create a new one or copy/symlink existing into `sites/` directory:

    cd sites/
    ln -s ~/path/to/your/jekyll-site jekyll-site

## Requirements

Mister Hyde is build using [Sinatra][sinatra] and read/writes data directly from the files in the Jekyll site directory, no external database is needed. Look at the Gemfile, it really is extremely boring.

It does however rely on [Git][git] and at this point expects the Jekyll sites to be checked into a git repository.

## Features

Completed features at this point is:

 * Create/Edit Posts

## Roadmap

Upcoming features in a prioritized list:

 * Delete Post
 * Git integration ( changes are committed )
 * Create new Jekyll site
 * Deploy functionality ( changes are pushed and/or `jekyll build` )
 * Create/Edit/Delete Pages

Future features in a non-prioritized list:

 * File management ( [Jekyll static files][jekyll-files] )
 * A better markdown editor
 * Authors/editors build-in ( authentication etc. )
 * Background running tasks

## Ideas/thoughts/bugs etc.

Please create an issue :)

[jekyll]:       http://jekyllrb.com/
[jekyll-files]: http://jekyllrb.com/docs/static-files/
[sinatra]:      http://www.sinatrarb.com/
[git]:          https://git-scm.com/