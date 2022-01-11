# Ansible-Windows-Linux
Ansible Automation Windows and Linux

pip3 install ansible pywinrm

### Run

ansible-playbook -i hosts windows_simple_playbook.yml

or only same Tags

ansible-playbook -i hosts install-choco.yml --tags "copy, service"
