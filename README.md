# Ansible Windows Server 2022 
## Configure a Microsoft Server 2022 machine to be (https://www.cisecurity.org/cis-benchmarks/) compliant

### Based on [ CIS Microsoft Windows Server 2022 v2.0.0 - 04-14-2023 ](https://www.cisecurity.org/cis-benchmarks/)

## Technical Dependencies:**

- Windows 2022 - 
- Running Ansible/Tower 
- Python3 Ansible run environment
- passlib (or python2-passlib, if using python2)
- python-lxml
- python-xmltodict
- python-jmespath
- pywinrm

## Execution:

    Run the playbook with the appropriate inventory file

    ansible-playbook site.yml -i inventory.ini


## Ansible Vault

To securely store the vault_postgresql_password, use Ansible Vault:

Regular Password Rotations: Implement a policy for regular password rotations to
 minimize the impact of potential compromises.

ansible-vault encrypt_string 'super_secure_password' --name 'vault_postgresql_password'
