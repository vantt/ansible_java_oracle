How to install
--------------

    ansible-galaxy install -r requirements.yml

with the content of requirements.yml
    
    
    # requirements.yml
    
    - src: https://github.com/vantt/ansible_java_oracle.git
      version: master
      name: java_oracle_role

How to use
----------

    # playbook.yml
    
    - hosts:  all 
      sudo: yes
      gather_facts: true
      roles:
        - { role: java_oracle_role }
