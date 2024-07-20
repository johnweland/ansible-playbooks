# Docker Swarm

The goal of this playbook it to take N number of VMs and provision X manager nodes and Y worker nodes

- role: 'install-prerequisites' works. 
- role: 'setup-docker-swarm' mostly works; need to figure out how to better use vars or hostvars to be able to a docker label of a given "size" to the appropriate node
- role: 'configure-glusterfs' is untested.
- role: 'leave-swarm' not intended to be used except as a tool for torubleshooting; comenting out other roles and uncommenting this will allow you to reset the docker swarm.