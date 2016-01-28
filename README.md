# ansible_endTB
ansible playbook to install bahmni(endTB) on a freshly installed centOS

Install bahmni on a test server

cd /tmp

git clone https://github.com/PIH/ansible

cd ansible

ansible-playbook -e "target=localhost" test


Run playbook on a remote server
-------------------------------

ansible-playbook -u root --extra-vars="target=IP_Address" remote_test -k
