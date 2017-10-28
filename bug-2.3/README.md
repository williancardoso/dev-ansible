## Running
```
ansible-playbook site.yml -i all
```

Observation: This code return the error bellow when using ansible version 2.3. Using ansible version 2.4, it's work! :)
```
fatal: [127.0.0.1]: FAILED! => {"failed": true, "msg": "The conditional check 'item.value.url_modulo is defined' failed. The error was: error while evaluating conditional (item.value.url_modulo is defined): 'ansible.vars.unsafe_proxy.AnsibleUnsafeText object' has no attribute 'value'\n\nThe error appears to have been in '/media/wvcardoso/hd_share/sync/repos_git/teste/ansible/bug/files.yml': line 17, column 3, but may\nbe elsewhere in the file depending on the exact syntax problem.\n\nThe offending line appears to be:\n\n\n- name: Download modules\n  ^ here\n"}
```

