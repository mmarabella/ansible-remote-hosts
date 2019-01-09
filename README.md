This repo contains two playbooks, test_connection.yml and test_pip.yml.
test_connection.yml uses the debug module to verify the connection to the remote hosts.
test_pip.yml uses the pip module to install ansible on the localhost and two remote hosts (personal macbooks).

Sensitive information is encrypted with ansible-vault, so the playbooks can only be run with
`ansible-playbook -i hosts test_connection.yml --ask-vault-pass`
