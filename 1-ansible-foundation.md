# Red Hat Delivery Specialist - Cloud Automation 
# Red Hat Ansible Automation Foundations 

# Ansible By RedHat 

  * Simple automation language. Infra as a code in playbook
  * Automation engine that runs ansible playbook
  * Ansible Tower - Enterprise framework control, manage, secure ansible with UI & REST api
  * Simple (readable) -> Powerful (App deploy) -> Agentless
  * Config management, App deploy, CD, provision, Security & compliance
  * It can be installed from EPEL, APT, PyPi, Sources from github
  * Playbooks - Plain text YAML describes the desired state of something
  * variables - Playbook files, inventories, Command line, Discovered variable
  * Inventories - Static list of servers, range of IP, Dynamic list from AWS, Azure, GCP
  * Playbooks - Contains play -> contains tasks -> tasks call modules.
  * Task run sequentially. Handlers are trigerred by tasks it will execute once at the end of task
  * Roles - Special kind of playbook. Self contained with variable, templates & supporting files
  * Ways to execute playbook - Ad-hoc, Playbook, Ansible tower
  * Ad-hoc - ansible web -m ping
  * playbook - ansible-playbook my-playbook.yml
  * Ansible Tower - UI control
  * Check mode - ansible-playbook -C my-playbook.yml - It will not execute the command & but it will check
  * Ansible tower - expands automation to the enterprose level
  * Ansible tower - control, schedule, knowledge, RBAC,simple, powerful,provide API to achieve CI/CD
  * Ansible tower needs - 64 bit linux machine, 2GB RAM, 4GB disk
  * Ansible Galaxy - Source for community & vendor provides playbooks
  * Galaxy roles are directly usable with little modification

LAB:

  * ansible web -b -m yum -a "name=httpd state=present"
  * ansible web -b -m service -a "name=httpd state=started"