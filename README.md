# Ansible playbooks for my raspi

## bootstrap.yml

This playbook expand the filesystem, optimize some kernel params (disable hdmi because of power saving etc.), basic security stuff (system update, ssh settings) and user provisioning.

### Requirements

    ansible-galaxy install -r requirements.yml

### Usage

    ansible-playbook pi-config-fs.yml -i hosts -k

    ansible-playbook pi-config.yml -i hosts -k
    
    ansible-playbook pi-secure-ssh.yml -i hosts

    ansible-playbook pi-purge.yml -i hosts

# License

MIT

