
# inventory INI

web1 ansible_host=server1.domain1.com ansible_connection=ssh ansible_ssh_pass=P@&sw
db ansible_host=server2.domain1.com ansible_connection=winrm ansible_ssh_pass=P@&


Variables use Jinja2 templating  
Fenced Code Blocks follows


        msg: "Username : {{ user.name }},  Password:{{ user.password }}"


Variable precendence:  
Host level variable has higher precedence than group level variable  
Play vars has higher precedence than Host level variable  
Extra vars has the highest precedence
https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_variables.html#understanding-variable-precedence

```
1. command line values (for example, -u my_user, these are not variables)
2. role defaults (as defined in Role directory structure) 1
3. inventory file or script group vars 2
4. inventory group_vars/all 3
5. playbook group_vars/all 3
6. inventory group_vars/* 3
7. playbook group_vars/* 3
8. inventory file or script host vars 2
9. inventory host_vars/* 3
10. playbook host_vars/* 3
11. host facts / cached set_facts 4
12. play vars
13. play vars_prompt
14. play vars_files
15. role vars (as defined in Role directory structure)
16. block vars (only for tasks in block)
17. task vars (only for the task)
18. include_vars
19. set_facts / registered vars
20. role (and include_role) params
21. include params
22. extra vars (for example, -e "user=my_user")(always win precedence)a

```

| Header 1 <b>| Header 2 |<b>
