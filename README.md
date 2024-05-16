frontend-app
=========

Role for frontend (react js) application deployment from http url or local fs.

Role Variables
--------------

To do

Example Playbook
----------------
```
- hosts: servers
  become: yes
  gather_facts: yes

  vars:
    frontend_app_name: "frontend-app"
    frontend_app_home_dir: "/var/www/ui/content/"
    frontend_app_archive_source: "local"
    frontend_app_archive_local_path: "../files/{{ frontend_app_name }}.tar.gz"

  roles:
    - frontend-app
```

