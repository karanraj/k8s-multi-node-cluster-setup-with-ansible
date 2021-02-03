# This is Ansible Automated program for setting up Kubernetes Multi Node Cluster
### For this you have to launch first AWS instance at least 2
### 1. Master Node
### 2. Slave Node(Worker Node)

**Here I've Created two Role And one playbook**
* k8s-master *For Configuring Master Node*
* k8s-slave *For Configuring Slave Node or Worder Node*
* playbook.yml *To run both roles*

**It Also Contain hosts and ansible.cfs files*
* hosts *This is a Inventory Which Contains All the hosts*
* ansible.cfg *This Contains All The Configuration For Ansible To Run on Remote System*

###### Then update IP's of two instances in hosts file under correct hostgroup

**Now you are good to go**

### Run playbook.yml
