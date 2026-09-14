# Bandit Level 13

## Goal
Use the private SSH key to log in as bandit14.

## Commands
```bash
exit
scp -P 2220 bandit13@bandit.labs.overthewire.org:/home/bandit13/sshkey.private .
chmod 600 sshkey.private
ssh -i sshkey.private bandit14@bandit.labs.overthewire.org -p 2220
```

## Key concepts
- Level 13 focuses on learning how to use Linux commands and basic cybersecurity/networking concepts.
- Use `man <command>` or `<command> --help` when you need command details.
