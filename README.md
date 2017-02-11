# vagrant-thingmonger

This is a virtual machine for [thingmonger](https://github.com/smoldata/thingmonger). If you aren't planning on doing software development on Thingmonger you can safely ignore this. This lives in its own separate repo because Thingmonger should be able to run without Vagrant just fine. This is just a quick way to bring up a Linux-y dev machine.

* Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
* Install [Vagrant](https://www.vagrantup.com/downloads.html)
* Setup your Vagrant machine:

```
mkdir /usr/local/smoldata
cd /usr/local/smoldata
git clone git@github.com:smoldata/thingmonger.git
git clone git@github.com:smoldata/vagrant-thingmonger.git
cd vagrant-thingmonger
vagrant up
```

## Setup Thingmonger

```
vagrant ssh
cd /usr/local/smoldata/thingmonger
make setup
```

You will be prompted with some configuration questions:

* Accept the defaults for unattended upgrades
* Choose a password for your Certificate Authority (you will be prompted to enter it again)
* Choose a root MySQL password
* Enter your root MySQL password when prompted

## Load it up in a browser

If everything goes as planned, you should be able to load up https://dev.thingmonger.org/ in your browser.
