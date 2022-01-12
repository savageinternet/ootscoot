# ootscoot

This repository contains the Octopress installation for our Oot 'n' a'scoot blog,
which chronicles our trip across America on our 300cc Vespa.

## Installation

    # clone the repo
    git clone https://github.com/savageinternet/ootscoot.git
    cd ootscoot

    # install dependencies
    brew update
    brew install rbenv
    brew upgrade ruby-build
    rbenv install 2.5.0
    rbenv local 2.5.0
    gem install octopress
    gem install bundler
    rbenv rehash

    # install more dependencies
    cd ootscoot.savageinter.net
    ~/.rbenv/shims/bundle

    # create a new post
    octopress new post "<post title>"

## Deployment

To test that everything works as expected, you can serve it locally:

    jekyll build
    jekyll serve
    # now visit http://localhost:4000 in your browser

When you're ready to deploy:

    octopress deploy

You will first need the `_deploy.yml` config file, which is not committed to
this repository - ask another blog maintainer.
