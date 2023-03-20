# r53
Ansible role for aws route 53

# Requierments

amazon.aws collection
````
    ansible-galaxy collection install amazon.aws
````
boto3
````
    pip3 install boto3
````

# Example Playbook
````
---
- name: Route 53
  hosts: localhost
  environment:
    AWS_ACCESS_KEY: "{{ Access_key_ID }}"
    AWS_SECRET_KEY: "{{ Secret_access_key }}"
    AWS_EC2_REGION: "{{ aws_region }}"

  # tasks: 
  
  roles:
    - r53

````
