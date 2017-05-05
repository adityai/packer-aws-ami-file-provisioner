# packer-aws-ami-ansible

The project has a packer template for creating an AWS AMI, a shell script for installing Ansible on the AMI, an Ansible playbook to install nginx on the AMI, an app folder and a ToUpload folder with nginx.conf and app-supervisor.conf.

## Pre-requisites
Add local environment variables for your AWS Account.

`export AWS_ACCESS_KEY_ID=<YOUR_AWS_ACCESS_KEY_ID>`

`export AWS_SECRET_ACCESS_KEY=<YOUR_AWS_SECRET_ACCESS_KEY>`

## Build

`packer build aws-ami-ansible-fileProvisioner.packer`

Optionally, build with debug enabled so Packer pauses after every step.

`packer build -debug aws-ami-ansible-fileProvisioner.packer`
