# ansible
Main assigments on Ansible Course

FOR PART1

to execute users.yml use the sentence:

ansible-playbook users.yml --ask-vault-pass

On promt introduce: secret

It should execute without any issues

FOR PART2

Part2 is using a roles structure so to execute simply run the main playbook:

ansible-playbook site.yml
