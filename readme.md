# Example project using Ansible
This project is a simple way to show how ansible and cloudformation can work together to setup hardware and configure the os and installed features. 

This example will launch a autoscaling set of instances and then contact github.com and pull the runbook you can see in here. The ELB is
setup to run as an internal elb. When inputing the cfn parameters, all can be left as default, with the exception of the following:
* SubnetList = Select one or more subnets that are internal (behind a nat)
* EBSRootType = select one, to keep price slow use standard
* KeyPairName = select a key pair so you are able to ssh onto the box if required
* VPCId = The VPC ID that the subnets you selected exist within


