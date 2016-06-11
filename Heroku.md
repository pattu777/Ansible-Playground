# Ansible-Playground
I recently bought a droplet from DigitalOcean. This repo contains Ansible playbooks that I used to customize the new server.

### Tasks

- Install packages.
- Setup a Django App.

### Prerequisites

- Ansible installed on your local system.
- Public SSH key copied to the remote server.
- Passwordless setup for a user with sudo privilleges.
- Provide the ip address of the server in hosts file.

#### Developing

Clone the repo and run the playbook.

```bash
$ git clone --recursive git@github.com:pattu777/Ansible-Playground.git
$ cd Ansible-Playground
$ ansible-playbook -i hosts setup.yml
```