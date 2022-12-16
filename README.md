# marvin
Automated resurrection of marvin

The purpose of this repo is to create a good sceleton of deploying single or multiple WordPress websites using nginx, php8 and mySQL at their latest versions.

My current setup is a manual configuration of couple websites that makes my life harder. The final decision to migrate to Ansible was because I can't migrate to PHP8.x, because I'm on Ubuntu 18.04 LTS. One last thing - never use ISPConfig.


Structure:
* Infrastructure as a Code - terraform to create a DO droplet
* Configuration management - Ansible
* Monitoring - grafana with logstash
* docker for various projects incl. portainer and heimdall
* container orchestration with kubernetes
* secrets management with HashiCorp Vault
* backup solution - bash and hope for the best

# Too complicated?

Maybe it is, maybe it isn't. That's my job so why not implement the best practices on my long suffering for best practices VPS? I have experience with all the technologies but never had the chance to start from the beginngin so I've found an scapegoat. Sorry, `marvin`.
