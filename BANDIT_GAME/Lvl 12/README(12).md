# Bandit Level 12

## Goal
Repeatedly identify and extract the compressed/archive file. Start by reversing hex.

## Commands
```bash
mkdir /tmp/bandit12
cp data.txt /tmp/bandit12/
cd /tmp/bandit12
xxd -r data.txt data
file data
# Rename/extract according to the type reported by file.
# Gzip: mv data data.gz && gzip -d data.gz
# Bzip2: mv data data.bz2 && bzip2 -d data.bz2
# Tar: mv data data.tar && tar -xf data.tar
# Run file after every extraction until ASCII text, then cat it.
```

## Key concepts
- Level 12 focuses on learning how to use Linux commands and basic cybersecurity/networking concepts.
- Use `man <command>` or `<command> --help` when you need command details.
