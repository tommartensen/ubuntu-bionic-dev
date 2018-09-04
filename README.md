# ubuntu-xenial-dev
> The only repository you need to setup your local development machine from scratch, reproducible!

* [I want that too](#i-want-that-too)
* [I want to add a command or program to the default setup](#i-want-to-add-a-command-or-program-to-the-default-setup)

## I want that too
### 1. Prerequisites
Not so much:
* Git (Host, obviously) or other means to download the content of this repo.
* Vagrant (Host)
* VirtualBox (Host)
### 2. Installation
Run `vagrant up`. That should be it.
If anything fails or you changed the configuration or playbooks, run `vagrant up --provision`.
Et voilà: VirtualBox opens the GUI with a login window and after a short moment, you're good to go.
> Password? You should really try vagrant 😉
#### What does it do?
> In a nutshell: Taking the configuration from the `Vagrantfile`, spinning up a virtual machine, installing ansible, running the playbook on the virtual machine against the virtual machine, installing updates and some important compilers/developer tools.

### 3. Customization
* Change Keyboard Layout
* Change your password (Hint: `passwd` is your friend)
* [Setup Git(hub) access](https://help.github.com/articles/connecting-to-github-with-ssh/)
* [Open additional ports](https://www.vagrantup.com/docs/networking/forwarded_ports.html)
### 4. Usage
You can spin the machine up with VirtualBox (with GUI) or `vagrant resume` if you suspended your machine.
Consequently, you may interact with the machine via GUI or login via ssh with `vagrant ssh`
### 5. How to remove all of it?
`vagrant destroy` and confirm. Be very sure about this.

## I want to add a command or program to the default setup
You are always installing something else after spinning up the box and wonder how to include this?
**Go no further**: Open a new issue, implement it on your own and open a PR, fork the repository, basically, [whatever you feel like](LICENSE.md).
Just make sure to not commit any secret keys and keep the project reproducible!

### You're welcome!
