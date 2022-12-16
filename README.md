# marvin
Automated resurrection of marvin

The purpose of this repo is to create a good sceleton of deploying single or multiple WordPress websites using nginx, php8 and mySQL at their latest versions.

My current setup is a manual configuration of couple websites that makes my life harder. The final decision to migrate to Ansible was because I can't migrate to PHP8.x, because I'm on Ubuntu 18.04 LTS. One last thing - never use ISPConfig.


Structure:
* Infrastructure as a Code - terraform to create a DO droplet
* Configuration management - Ansible
* Monitoring - grafana with logstash
* Containers:
	* docker for various projects incl. portainer and heimdall
	* container orchestration with kubernetes
* Secrets management with HashiCorp Vault
* Backup solution - bash and hope for the best
* CI/CD - GitHub actions including container and leaking secrets scanning, DAST, SAST, IAST and automatic deployments of approved PR

# Too complicated?

Maybe it is, maybe it isn't. That's my job so why not implement the best practices on my long suffering for best practices VPS? I have experience with all the technologies but never had the chance to start from the beginngin so I've found an scapegoat. Sorry, `marvin`.

# btw who is `marvin`?

Marvin is named after the always suffering humanoid from Douglas Adams' The Hitchhiker's Guide to the Galaxy and my VPS where https://nedko.info and couple of other projects lives. More info and his lifetime [can be found here](https://www.nedko.info/marvin/).
