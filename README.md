# Ansible Role: ec2_k8s_Master
=========

A simple Ansible role for creating a Ks8 Slave on AWS ec2 instance.


It will install the following:-
------------
  
  ansible
  boto
  boto3
  
Role Name
=========

A brief description of the role goes here.
This role is used for setting up the Kubernetes Cluster Slave on AWS public cloud. This role can also be used on Amazon Linux 2 ami having t2.micro instance type or any higher insatance type.

Requirements
------------

Pre-requisite for using this role is you must have yum configured if you are using Rhel OS or if any other OS installing tool should be available.

Attention
---------

As when we create any insytance we give tags. So both the python script will Create inventory groups using tags modify as you use them in your environment.

For getting the group of tags so to your /etc/ansible/host directory use this command:- "python3 ec2.py" 
Now you can see all your instance ip's with their following tags.

You can also use these tags.
In my case I used it as follows in ec2_instances_facts.yml.

    hosts: tag_Name_Production
     
    hosts: key_mykey
     

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles. In this role there is no variable to define only run this role.


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

---
- hosts: localhost
  
  gather_facts: no

  roles:

    - /path/ec2_k8s_Slave

...
License
-------

BSD

## Contributing

Issues, feature requests, ideas are appreciated and can be posted in the Issues section.


Author Information
------------------
LinkedIn: https://www.linkedin.com/in/komalsuthar

![](https://visitor-badge.glitch.me/badge?page_id=24-komal.ec2_k8s_Slave)


