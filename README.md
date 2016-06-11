# Ansible-Playground
I recently bought a droplet from DigitalOcean. This repo contains Ansible playbooks that I wrote to customize the new server. More detailed information can be found on my blog [chinmayapatanaik.com](chinmayapatanaik.com).

### Tasks

- Install packages.
 * Git
 * zsh
 * oh-my-zsh
 * vim
 * tmux
 * python-pip
 * python-virtualenv
 * Atom Editor
 * Sublime Text Editor
 * vlc
 *  
- Copy SSH public key to Github.
- Copy SSH Key to a remote server

### Prerequisites

- Ansible installed on your local system.
- Public SSH key copied to the remote server.
- Passwordless setup for a user with sudo privilleges.
- Provide the IP address of the server in hosts file.

#### Developing

Clone the repo. Modify inventory file and the playbook with information of remote server. Finally run the playbook as shown below.

```bash
$ git clone --recursive git@github.com:pattu777/Ansible-Playground.git
$ cd Ansible-Playground
$ ansible-playbook -i hosts setup.yml
```
