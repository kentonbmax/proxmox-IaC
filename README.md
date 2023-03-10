# proxmox-IaC
Proxmox examples using Terraform and Ansible

## Getting Started
1. Grab your ansible ssh public key. Put it in a file, `~/.ssh/ansible.pub` on proxmox
1. Transfer the contents of the script to your proxmox using the following:
   `wget https://raw.githubusercontent.com/kentonbmax/proxmox-IaC/main/scripts/cloud-template.sh`
   `wget https://raw.githubusercontent.com/kentonbmax/proxmox-IaC/main/scripts/setup-ansible-image.sh`
1. Give permission `chmod +x *.sh`
1. Run `./cloud-template.sh`
1. (Optional) Running Ansible
   1. Create in the home directory a 4096 rsa key for ssh in a file named ansbile `ssh-keygen -t rsa -b 4096`
1. GUI - CloudInit tab set networking DHCP = true
1. Right click 9001 and convert to template. 
1. Ready to clone. 
   
## References and motivations
- [Inject Keys](https://www.cyberciti.biz/faq/how-to-add-ssh-public-key-to-qcow2-linux-cloud-images-using-virt-sysprep/)
- [Proxmox Templates](https://pve.proxmox.com/wiki/VM_Templates_and_Clones)
- [ansible cloud image](https://ronamosa.io/docs/engineer/LAB/proxmox-cloudinit/)

## Other Work
[Learn Typescript Node Templates](https://learntnt.com)

