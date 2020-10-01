# Project
Accomplishment
Description of the Topology
The main purpose of this network is to expose a load-balanced and monitored instance of DVWA, the D*mn Vulnerable Web Application.
Load balancing ensures that the application will be highly _____, in addition to restricting _____ to the network.

TODO: What aspect of security do load balancers protect? What is the advantage of a jump box?

Integrating an ELK server allows users to easily monitor the vulnerable VMs for changes to the _____ and system _____.

| Name     	| Function  	| IP Address 	| Operating System 	|
|----------	|-----------	|------------	|------------------	|
| Jump Box 	| Gateway   	| 10.1.0.4   	| Linux            	|
| Web-1    	| Container 	| 10.0.0.9   	| Linux            	|
| Web-2    	| Container 	| 10.0.0.10  	| Linux            	|
| Web-3    	| Container 	| 10.0.0.11  	| Linux            	|
| Red-Elk  	| Kibana    	| 10.0.0.4   	| Linux            	|


Access Policies
The machines on the internal network are not exposed to the public Internet.
Only the Jumpbox and Elk machine can accept connections from the Internet. Access to this machine is only allowed from the following IP addresses:



Machines within the network can only be accessed by Web-1,2,3_.


A summary of the access policies in place can be found in the table below.

| Name     	| Publicly Accessible 	| Allowed IP Addresses 	|
|----------	|---------------------	|----------------------	|
| Jump Box 	| Yes                 	| 52.143.70.170        	|
| Web-1    	| No                  	| 10.1.0.9             	|
| Web-2    	| No                  	| 10.1.0.10            	|
| Web-3    	| No                  	| 10.1.0.11            	|
| Red-Elk  	| Yes                 	| Personal       	|

Elk Configuration
Ansible was used to automate configuration of the ELK machine. No configuration was performed manually, which is advantageous because

This configures the target VM (the machine being configured) to use more memory. The ELK container will not run without this setting.

You will want to use Ansible's sysctl module and configure it so that this setting is automatically run if your VM has been restarted.
The most common reason that the ELK container does not run, is caused by this setting being incorrect.
Ansible sysctl


Using the Playbook

The file is filebeat-config.yml will be copied in to webservers.
Update the hosts file to note what machiene will be included. Use the webserves list to add machienes for filebeat and metricbeat and Elk server has its own list.
http://23.98.145.100:5601/app/kibana#/home/tutorial_directory/logging


