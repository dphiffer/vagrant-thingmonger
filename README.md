# vagrant-thingmonger

This is a virtual machine for [thingmonger](https://github.com/smoldata/thingmonger). If you aren't planning on doing software development on `thingmonger` you can safely ignore this. This lives in its own separate repo because `thingmonger` should be able to run without Vagrant just fine. This is just a quick way to bring up a Linux-y dev machine.

* Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
* Install [Vagrant](https://www.vagrantup.com/downloads.html)

```
mkdir /usr/local/smoldata
cd /usr/local/smoldata
git clone git@github.com:smoldata/thingmonger.git
git clone git@github.com:smoldata/vagrant-thingmonger.git
cd vagrant-thingmonger
vagrant up
```
