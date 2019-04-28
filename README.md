# ansible-cisco-ios-management
This repository provides playbooks for managing Cisco IOS devices

<p align="center">
  <a href="#Getting-Started">Getting Started</a> •
  <a href="#Playbooks">Playbooks</a> •
  <a href="#Related">Related</a> •
  <a href="#Authors">Authors</a>
</p>

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

## Playbooks

### Change MGCP Agent
```yaml
tasks:
     - ios_config:
          provider: "{{login_info}}" 
          lines:
            - mgcp call-agent 10.0.0.10
          before: "no mgcp call-agent 10.0.0.9"  
       
     - ios_config:
          save: yes
          provider: "{{login_info}}"
```

## Related

* [Ansible](https://www.ansible.com) - Configuration Management
* [AWX](https://github.com/ansible/awx) - Configuration Management
 

## Authors

* **Javier Baltar** - *Initial work* - [GitHub](https://github.com/JavierBaltar)
