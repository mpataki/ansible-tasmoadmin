
# ansible-tasmoadmin

[![Build Status](https://travis-ci.org/mpataki/ansible-tasmoadmin.svg?branch=master)](https://travis-ci.org/mpataki/ansible-tasmoadmin)

This role sets up [TasmoAdmin](https://github.com/reloxx13/TasmoAdmin) on a raspberry pi, and is largely adapted from [this guide](https://github.com/reloxx13/TasmoAdmin/wiki/Guide-for-Ubuntu-Server-16.04#set-full-readwrite-access-on-varwwwtasmoadmintmp-and-varwwwtasmoadmindata).

The resulting TasmoAdmin install will run on port 9999.

## Requirements

Really this should work on any debian based system, but has been tested on a Raspberry Pi running Hassbian.

## Role Variables

- `tasmoadmin_version`
  - Defaults to v1.6.0

## Example Playbook

```yml
    - hosts: pi
      roles:
         - role: mpataki.tasmoadmin
```

## License

MIT
