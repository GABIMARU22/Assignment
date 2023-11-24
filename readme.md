Three-Tier Web Application Infrastructure
This project implements a three-tier web application infrastructure comprising a load balancer, application servers, and a database server using Vagrant and Ansible.

Getting Started
These instructions will help you run this project on your local machine for development and testing purposes.

Prerequisites
You must have the following installed on your machine:

Vagrant
VirtualBox
Ansible
Directory Structure
Copy code

├── Vagrantfile
├── ansible.cfg
├── playbook.yml
├── roles
│   ├── app
│   │   └── tasks
│   │       └── main.yml
│   ├── db
│   │   └── tasks   
│   │       └── main.yml
│   └── lb
│       └── tasks
│           └── main.yml
├── README.md
Key files and directories:

Vagrantfile: Vagrant configuration file for defining VMs.
playbook.yml: Main Ansible playbook to configure servers.
roles/: Directory containing Ansible roles to configure each component.
README.md: This instruction file.
Running the Application
Follow these steps to run the application:

Clone this repository to your local machine.

Change into the project directory.

Run vagrant up to create the VMs and configure them using Ansible playbook.

Once Vagrant completes provisioning, access the load balancer IP on port 80 in your browser:

http://192.168.33.13

This will access the test application via the load balancer, demonstrating the configured three-tier infrastructure.

Run vagrant destroy -f to delete the VMs once done testing.
Author
Hrishikesh Patne
hrishikeshpatne2@gmail.com.com

Let me know if you need any other details in the README!
