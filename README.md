# Packer
Packer for Vsphere

this is a pipeline project that would make Ubuntu templates for vcenter. I will be using Ansible to provision these templates.

the structure is
 - JSON packer template that will run the pipeline.
 - Variables file that I will use to fill the missing fields in the Template.
 - Ansible playbooks

make sure that all these files are in the same directory, and Packer in /usr/bin to run its commands globally.
I will be using "ansible-local" because I dont want to run the playbooks from my mac. too much headache.
I will be installing Ansible on the Template and copy any files and Installers I need to the /tmp/ dir there.
