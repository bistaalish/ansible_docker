# Ansible Playbook: Install Vagrant with Libvirt and Docker on Debian 12

This Ansible playbook automates the installation of Vagrant with Libvirt, Docker, and Docker Compose on a Debian 12 system. It also provides an option to create a Docker user.

## Prerequisites

- Ansible installed on your control machine.
- A Debian 12 target machine.

## Usage

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/your_username/ansible-debian-docker.git
   cd ansible-debian-docker
   ```
2. Customize variables in the inventory file (inventory) as needed for your environment:

    -**`DOCKER_USERNAME`**: The name of the Docker user to be created.

    -**`DOCKER_USER_SHELL`**: The shell for the Docker user.

    -**`DOCKER_PASSWORD`**: The password for the Docker user.

3. Run the Ansible playbook:

    ```bash
    ansible-playbook  playbook.yml
    ```