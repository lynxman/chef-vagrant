chef-vagrant
============

Chef Vagrant stuff, some random weekend experiment with librarian chef

It uses Omnibus to install chef-solo on top of a base install image (Ubuntu 12.04 LTS 64 bits)

The files
---------
*Cheffile* => It has all the cookbooks you want to run
*cookbooks* => Directory where the cookbooks will download, don't put any of your cookbooks here
*roles* => Directory where the roles live, I created a `test1.json` as an example
*site-cookbooks* => Directory to put your recipes and try weird experiments

Preparation
-----------
You'll need
* 1 Vagrant (http://vagrantup.com)
* 1 Virtualbox (http://www.virtualbox.org)

Stir your Vagrant by adding the needed plugins
`vagrant plugin install vagrant-librarian-chef`
`vagrant plugin install vagrant-omnibus`

Your Vagrant recipe
-------------------
Copy the files inside the `vagrant` directory of this repo into a directory where you'll setup your vagrant env for this.
Once you got this create a directory `chef` inside with the full content of this repo (maybe a `git clone`?)

Modify the roles or create roles of your choice for the fun of it

Starting it up
--------------
Run `vagrant up` to boot up the service, with vagrant ssh you should be easily in once all is finished \o/

Have fun!

