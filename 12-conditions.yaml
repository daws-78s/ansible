- name: conditions
  hosts: web
  become: yes
  tasks:
  - name: check user exists or not
    ansible.builtin.command: id expense
    register: USER
    ignore_errors: true

  - name: print user information
    ansible.builtin.debug:
      msg: "User info: {{USER}}"

  - name: create user
    ansible.builtin.command: useradd expense
    when: USER.rc != 0 #condition

  - name: say Hello
    ansible.builtin.debug:
      msg: "Hello"