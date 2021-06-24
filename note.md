```
ansible-galaxy collection install community.routeros

```

```
➜ ansible ansible -i hosts router  -m routeros_command -a 'commands="/system resource print"'
[WARNING]: Platform linux on host 192.168.88.1 is using the discovered Python interpreter at /usr/bin/python, but future installation of another Python interpreter could change the meaning of
that path. See https://docs.ansible.com/ansible/2.11/reference_appendices/interpreter_discovery.html for more information.
192.168.88.1 | SUCCESS => {
    "ansible_facts": {
            "discovered_interpreter_python": "/usr/bin/python"
        },
    "changed": false,
    "stdout": [
            "uptime: 4w22h3m\n                  version: 6.48.2 (stable)\n               build-time: Apr/09/2021 10:17:26\n         factory-software: 6.44\n              free-memory: 69.9MiB\n             total-memory: 128.0MiB\n                      cpu: ARMv7\n                cpu-count: 4\n            cpu-frequency: 716MHz\n                 cpu-load: 0%\n           free-hdd-space: 1808.0KiB\n          total-hdd-space: 15.3MiB\n  write-sect-since-reboot: 187368\n         write-sect-total: 1627625\n               bad-blocks: 0%\n        architecture-name: arm\n               board-name: hAP ac^2\n                 platform: MikroTik"
        ],
    "stdout_lines": [
            [
                        "uptime: 4w22h3m",
                        "                  version: 6.48.2 (stable)",
                        "               build-time: Apr/09/2021 10:17:26",
                        "         factory-software: 6.44",
                        "              free-memory: 69.9MiB",
                        "             total-memory: 128.0MiB",
                        "                      cpu: ARMv7",
                        "                cpu-count: 4",
                        "            cpu-frequency: 716MHz",
                        "                 cpu-load: 0%",
                        "           free-hdd-space: 1808.0KiB",
                        "          total-hdd-space: 15.3MiB",
                        "  write-sect-since-reboot: 187368",
                        "         write-sect-total: 1627625",
                        "               bad-blocks: 0%",
                        "        architecture-name: arm",
                        "               board-name: hAP ac^2",
                        "                 platform: MikroTik"
                    ]
                        ]
}
```
