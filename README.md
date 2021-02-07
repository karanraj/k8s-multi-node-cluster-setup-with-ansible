# This is Ansible Automated program for setting up Kubernetes Multi Node Cluster on AWS 
## This program will launch and configure
### 3. 3 AWS Instances
### 2. One Master Node
### 3. Two Slave Node(Worker Node)

**Here I've Created two Role And two playbook**
* aws_launch.yml *Playbook to Launch One master and two slave node on AWS*
* k8s-master *Role For Configuring Master Node*
* k8s-slave *Role For Configuring Slave Node or Worder Node*
* playbook.yml *Playbook To run both roles*

**It Contains hosts and ansible.cfg files**
* hosts *This is a Inventory Which is empty as of now and after launching 3 AWS Instances it will auto create two group containing master and slaves(worker nodes) IP as Managed Host*
* ansible.cfg *This Contains All The Configuration For Ansible To Run on Remote System*


**Now you are good to go**

### 1st run the aws_launch.yml to launch instances 
*Make sure that you have configured aws in your CLI for asw_access_key and aws_secret_key*
*and must use tag group:master for master instance and group:slave for slave instances*
### 2nd run the playbook.yml to configure master ans slave(worker node)
