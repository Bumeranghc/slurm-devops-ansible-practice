# slurm-devops-ansible-practice
Generate ssh key pair in 'files' directory and name it 'xpaste'

Run Vagrant with:

```
vagrant up
```

Connect to control node with:

```
vagrant ssh controlnode
```

Copy ansible directory and align file permissions

Run playbook with:

```
ansible-playbook playbook.yml -e "gitlabuser=<your_user_for_xpaste_repo>" -e "gitlabpassword=<your_password_for_xpaste_repo>" -e "xpaste_secret_key=<your_secret_key>" -e "xpaste_db_password=<your_db_pass>"
```