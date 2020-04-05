# hxl-standard-tools-stack/ansible

The hxl-standard-tools-stack/ansible provides a way to prepare the host that
will run the docker containers using Ansible.

## Usage

### Install dependencies

You need a host with Ansible installed, See [Installing Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html).

```
ansible-galaxy install -r requirements.yml
```

### Customize the hosts

Please copy the contents of inventories/etica.dev folder and customize to your
needs (in special, change the target host). All examples use the `hxl.etica.dev`
as a testing server.

### Running the playbooks

```bash
# This will run all playbooks
ansible-playbook -i inventories/etica.dev playbook.yml

# You can run just one part of the playbooks at time. Read the contents of the
# files at playbooks/ folder to more details. For example, this command will
# just do Ansible ping (to test if you are able to connect on the target host)

ansible-playbook -i inventories/etica.dev playbooks/ping-all.yml
```
