

Team: Purnesh Anugolu, Sai Aditya Thalluri, Sai Kiran Veera

Setup:
	- We implemented the Homework by using 3 Cloud VM servers purchased from linode.com
	- Hosts and their credentials are mentioned in the hosts file


Instructions:

Task1: Create playbook to write team names in /root/team.txt by using a common role

Run : ansible-playbook task1.yml

Output: It writes the team names to text file



Task2: Creating a mongo-replicate set on 3 VMs. 
Roles, tasks, handlers, templates and group_vars 
created to configure mongodb in each machine and enable replication.

Run: ansible-playbook task2.yml

Output: Installs mongodb in all VMs, enables replication initialization in primary node and creates collection. 
In secondary slave database, we will be able to see the collection created by primary. 


Extra credit: Created handler to restart the deamon service after the configuration is done in primary and secondary nodes. 
