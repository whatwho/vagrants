# Vagrant @ DiNa

## About

This vagrant box is for Digital Natives Ruby on Rails development. It's a box containing ALL the necessary stuff to be able to work on a DiNa project. It's a temporary solution, the future is to move the virtualization to Docker, and create application related containers.

## Installment

### Install prerequisitons

Vagrant needs a virtualization provider, we support virtualbox. Please download it from [here](https://www.virtualbox.org/wiki/Downloads).

Please also download vagrant from [here](http://downloads.vagrantup.com/)

### Clone this repository

`git clone git@bitbucket.org:digital_natives/vagrants.git`

### Chef installment

Chef is a ruby gem, therefore you need a Ruby on your host machine. The easiest way, if you install rvm and install a ruby version under it. When this box was created, chef 11.8.2 was the current version.

`gem install chef`

### Berkshelf installment

Berkshelf is a chef cookbook package handling system written in ruby. Berkshelf downloads all the necessary cookbooks and their dependencies.

Install berkshelf gem:

`gem install berkshelf`

Install berkshelf vagrant plugin:

`vagrant plugin install vagrant-berkshelf`

## Usage

### Start

`vagrant up`

### Stop

`vagrant halt`
