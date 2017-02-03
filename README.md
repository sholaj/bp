BP

Tasks
- Spin up a Linux Vagrant box of your choice
- Configure Vagrant to use Ansible as the provisioner
- Configure the box with an IP address available to the hosting OS
- Write playbook/playbooks to:
  i.   Install and start docker
  ii.  Build a docker container based on the official Alpine Linux container (library/alpine:latest)
  iii. Build the container so that nginx is installed and started
  iv.  Configure nginx to serve out some static “Hello World” content
  v.   Start the container as a micro service
  vi. At the end of the provisioning the URL to the web page should be available from the hosting OS
  vii. Write appropriate documentation in the repository to explain how someone cloning it should provision the Vagrant VM and access the web URL serving out the “Hello World”


Prerequisites - The setup was test on the version listed below

Install vagrant version 1.8.1
Install ansible 2.0.2.0

HOWTO

git clone git@git@github.com:sholaj/bp.git
cd bp/my-bp-project
vagrant status
vagrant up bp
vagrant ssh bp 
export DOCKER_HOST="tcp://192,168.50.4:2375"
ansible-container build
ansible-container run




TODO
ansible-container build failing with synatx error..Time constraints
script container build and run process


