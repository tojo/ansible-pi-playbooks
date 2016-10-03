# Ansible playbooks for my FHEM installation on a pi

This playbooks expand the filesystem, optimize some kernel params (disable hdmi because of power saving etc.), basic security stuff (system update, ssh settings), user provisioning and purge tons of X11 stuff.

### Requirements

    ansible-galaxy install -r requirements.yml

### Usage

	ansible-playbook fhempi-0-bootstrap.yml

    ansible-playbook fhempi-1-config-pi.yml

    ansible-playbook fhempi-2-secure.yml

# License

MIT

