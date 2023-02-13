# Ansible

### Automation of infrastructure construction with Ansible

* EC2 Construction
* RDS Construction
* Wordpress(Apache)
* Wordpress(nginx)
* Installing Jupyternotebook on EC2
* Installing GitLab on EC2

### Usage

1. Select the tasks you want to run from the `tasks` directory and specify them in `main.yml` with `include_tasks`.
1. Update variables in `vars.yml.
1. Enter the managed node to `hosts.ini`.
1. Execute the following command. Optionally, `-v` outputs the processing contents.

__Command__

```
ansible-playbook -i hosts.ini main.yml
```