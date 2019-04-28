<p align="center">
  <a href="#Getting-Started">Getting Started</a> •
  <a href="#Playbooks">Playbooks</a> •
  <a href="#Authors">Authors</a> •
  <a href="#related">Related</a> •
  <a href="#license">License</a>
</p>

# ansible-cisco-ios-management
This repository provides playbooks for managing Cisco IOS devices


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

## Playbooks

What things you need to install the software and how to install them

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

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes

## Built With

* [Ansible](https://www.ansible.com) - Configuration Management
* [AWX](https://github.com/ansible/awx) - Configuration Management
 

## Authors

* **Javier Baltar** - *Initial work* - [GitHub](https://github.com/JavierBaltar)


## License


## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc


```python
var editor = new tui.Editor({
    el: document.querySelector('#editSection'),
    initialEditType: 'markdown',
    previewStyle: 'vertical',
    height: '300px'
});
```
