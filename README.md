# Ansible Datadog Role

This Ansible playbook installs and configures the Datadog Agent. It utilizes the Datadog role to achieve this.

## Setup

### Requirements of Ansible Playbook

- Requires Ansible v2.6+.
- Supports most Debian and RHEL-based Linux distributions, macOS, and Windows.
- When using Ansible 2.10+ on Windows, requires the `ansible.windows` collection to be installed.

### Hosts file setup

* Create a file `hosts` in your home directory on your PC.
* Add the IP address of your hosts server(s) in the file `hosts`

### Installation

Execute this command on your PC (substituting the User ID for the server host as well as file name of the private key):

```ansible-playbook -i ~/hosts -u <user_id_on_server_host> --private-key=~/.ssh/<private_key_file> dd_agent.yml```
