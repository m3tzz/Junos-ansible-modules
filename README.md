
Juniper.junos Ansible Modules --> http://junos-ansible-modules.readthedocs.io/en/2.0.1/

################ To install the modules##########

Run this command below:
ansible-galaxy install Juniper.junos,2.0.1

############ How to run the playboox###############

First, go inside of the folder related with juniper devices model you want to made changes
e.g --> cd /Junos/ex

-t means the name of the tag you defined on your playbook
-e means the name of the tag you defined on your playbook to call a device or more then one device
--ask-vault-pass - provide the ansible-vault password to run playbook


ansible-playbook -i hosts ex.yaml -t add_vlanl3 -e ci_name=ex-sw1 --ask-vault-pass


ansible-playbook -i hosts ex.yaml -t add_vlanl3 -e ci_name=qfx-sw1 --ask-vault-pass
