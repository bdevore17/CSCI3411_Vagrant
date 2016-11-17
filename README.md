# CSCI 3411 Vagrant
Assignments in CSCI 3411 at George Washington Univeristy are graded in Ubuntu 14.04, so all students should make sure to test their assignments in it too. This repository allows students to test their assignments in Ubuntu 14.04 with extreme ease.

## Prerequisites
Before using this project, you must install the latest versions of [Vagrant](https://www.vagrantup.com/downloads.html) and [VirtualBox](https://www.virtualbox.org/wiki/Downloads).
### Installation
1. Clone this repository using `git clone` into the same parent directory as your CSCI 3411 assigments.
2. `cd` into this repository
3. Run `vagrant up`. This command with bring up a headless instance of Ubuntu 14.04 in VirtualBox. This can take a few minutes.
4. Run `vagrant ssh`. Once this commands completes, you will have access to Ubuntu via ssh.
5. Within the virtual machine, run `cd /CSCI3411`. You will now be inside the parent directory of this repository on you host machine. From here, you will be able to easily test all of your assignments.
6. When you are done testing, run `exit` and you will be returned to your host machine. Keep in mind however, that Ubuntu is still running.
7. To shutdown Ubuntu, run `vagrant halt` on your host machine. To delete Ubuntu, run `vagrant destroy`.
8. To bring Ubuntu back up at any time, simply run `vangrant up` on your host machine.

#### Running Xv6 With this Repo
Within your Xv6 repo (inside of your Vagrant VM), run `make qemu-nox`. This is should bring up Xv6 on your command line. To quit, use ctrl+a x.
