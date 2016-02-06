# Ansible playbooks for my raspi

## bootstrap.yml

This playbook expand the filesystem, optimize some kernel params (disable hdmi because of power saving etc.), basic security stuff (system update, ssh settings) and user provisioning.

### Requirements

    ansible-galaxy install -r roles

### Usage

    ansible-playbook pi-config.yml -i hosts -k
    
    ansible-playbook bootstrap.yml -i hosts -k

# License

MIT

