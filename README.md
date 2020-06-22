# Dev Env / Vagrant 101


#### What is an Env?
A location where code runs and data lives eg this laptop (not GitHub)

- Development
  - Python, SQL, HTML, CSS...
- Testing
  - Ensures functionality and quality
  - Has its own tools / infrastructure that dev environments lack
- Production


- Pipelines transfer code from dev --> test --> production

#### 4 Pillars of DevOps
Defines the role


1) Ease of use
  - Infrastructure needs to be easy to use for entire team

2) Flexibility
  - Allows ability to evolve

3) Robustness
  - 100% uptime
  - Fast deployment
  - Strength / Reliability of Infrastructure

4) Cost
  - Cap-ex & Op-ex
  - Cost of downtime
  - Cost of slow innovation
  - Cost of time to market
  - Cost of infrastructure


#### DevOps problems and solutions
- Product works on one machine but not another ???
- Testing environment set up, STANDARDIZED
	- Ensures functionality



## Vagrant & VirtualBox
- Combined allows for virtual machine (environment)


### VirtualBox
- VirtualBox is a general-purpose virtualization tool for x86 and x86-64 hardware, targeted at server, desktop, and embedded use, that allows users and administrators to easily run multiple guest operating systems on a single host.
- Manager

### Vagrant
- Vagrant is an open-source software product for building and maintaining portable virtual software development environments


1 - vagrant init <box>
	- Creates vagrantfile, config.vm.box = "base"
		- Convert base to box server:
			https://app.vagrantup.com/boxes/search
		- Create private network (public):
			config.vm.network "private_network", ip: "192.168.10.100"
			- Can go to ip in browser

2 - vagrant up
	- Starts up server, takes time

3 - vagrant ssh 
	- Enter machine
	- Same commands as git bash

- vagrant reload
- vagrant destroy
- exit


### nginx 

4 - sudo apt-get update -y
	- APT (package manager)
	- Gets and updates packages

5 - sudo apt-get install nginx -y
	- Install nginx 
	- -y = "say yes"

6 - sudo systemctl start nginx
	- starts nginx

7 - Go to hosturl