# Prometheus Node Exporter Installation with Ansible

This Ansible playbook automates the installation of Prometheus Node Exporter on multiple Ubuntu Virtual Machines. It allows you to specify the version of Node Exporter to use and uses username/password authentication to connect to the VMs.

## Prerequisites

- Ansible installed on your local machine 
- SSH access to the target Ubuntu VMs


## Setup Instructions

1. Clone this repository or copy the files to your local machine:
2. Update the `inventory.yml` file with your target Ubuntu VM IP addresses:
3. Modify the `vars/main.yml` file with your VM credentials and desired Node Exporter version:
4. (Optional) Adjust any other variables in `vars/main.yml` or `roles/node_exporter/defaults/main.yml` if needed.

## Usage

To run the Ansible playbook and install Node Exporter on your target VMs, use the following command:


ansible-playbook playbook.yml

## Verifying the Installation

After running the playbook:

1. SSH into one of your target VMs.
2. Check if the Node Exporter service is running
