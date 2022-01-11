# Ansible-Windows-Linux
Ansible Automation Windows and Linux

# Installacja na serwerze
pip3 install ansible pywinrm

### Run

ansible-playbook -i hosts windows_simple_playbook.yml

or only same Tags

ansible-playbook -i hosts install-choco.yml --tags "copy, service"


# Uruchomieniw WinRM na Hoscie docelowym

# Ansible
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://raw.githubusercontent.com/ansible/ansible/devel/examples/scripts/ConfigureRemotingForAnsible.ps1'))
