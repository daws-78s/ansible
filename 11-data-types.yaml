- name: data types
  hosts: localhost
  vars:
    Course: DevOps with AWS #string
    Tools: # list
    - Linux
    - Shell
    - Ansible
    Experience: # map or dictionary
      DevOps: 3 # number
      AWS: 2
      Docker: 1
    RealProject: true #boolean
  tasks:
  - name: print variables
    ansible.builtin.debug:
      msg: "Course: {{Course}}, Tools covered: {{Tools}}, Experience is: {{Experience}}, is real project: {{RealProject}}"