# Project Description
The objective is the design and implementation of a secure infrastructure
through the use of virtual machines. The implementation
will be realised through the configuration of a firewall and intrusion detection systems.
intrusion detection systems. It will also require the installation and configuration of
software capable of correctly filtering incoming and outgoing packets
according to the defined rules and policies. In addition, software will be configured to
monitoring and logging changes made to critical files on the system.
in the system. It must be possible to access from outside the functionalities provided
provided by the system, through an authentication mechanism. The infrastructure shall
be robust, i.e. able to prevent and resist different types of common attacks.

## Virtual Machine Installation Guide

To install the virtual machines that form the basis of the secure infrastructure, it is necessary to install software for running virtual machines, such as _VirtualBox_, on your computer.

The OVA files of the two virtual machines are available at the following OneDrive link: [link](https://univpm-my.sharepoint.com/:f:/g/personal/s1107326_studenti_univpm_it/EgCbgyeSVlJAsLq6-frnymIBja30dy-1lVXBz99MaxghoA?e=U6B6bF).

If you encounter problems when starting the machines, check that the network interfaces have been correctly detected and that the allocated resources are sufficient.

Once installed, the two machines can be started up and the entire system can be tested.

The first virtual machine, named **Dual-homed Host**, performs the tasks of a Screening Router and a Bastion Host. At start-up, the user can access one of two available accounts: 
* **screening**: account with root permissions, required for the implementation and management of policies and security for the entire infrastructure. It is reserved for the system administrator. The password to access this account is: univpm2223.
* **guest**: account without root permissions, set up for user access via SSH. The password to access this account is: guestscreening.

The second virtual machine, the **Client** machine, simulates the behaviour of a machine belonging to the internal network. At start-up, the user can access one of two available accounts:
* **client**: account with root permissions, needed to manage and control the files on the machine. It is reserved for the system administrator. The password to access this account is: groupotto.
* **guest**: Account without root permissions, set up for user access via SSH. The password for accessing this account is: guestclient.

Using these machines, it will be possible to carry out some tests on the infrastructure yourself. Examples of tests can be found in Chapter 4 of the PDF file.
