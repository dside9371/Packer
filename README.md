# Packer
Packer for Vsphere

This is a pipeline project that makes Ubuntu templates for vcenter. I will be using Ansible to provision these templates.

The structure is
 - JSON packer template that will run the pipeline.
 - Variables file that I will use to fill the missing fields in the Template.
 - Ansible playbooks

NOTE: Make sure that all these files are in the same directory, and Packer in /usr/bin to run its commands globally.
      I will be using "ansible-local" because I dont want to run the playbooks from my Mac (too much headache)
      I installed Ansible on the Template and copied any files and installers that I needed to the /tmp/ dir there.

Example command: 
        $ packer build -var-file variables.json ubuntu2004.json
