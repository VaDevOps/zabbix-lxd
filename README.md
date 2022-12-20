# Zabbix-LXD

## Overwiew

For Zabbix version: 6.2 and higher  
The template to monitor LXD engine by Zabbix.
Most of the metrics are collected in one go, thanks to Zabbix bulk data collection.

Template `LXD by Zabbix agent ` — collects metrics by polling zabbix-agent2.

This template was tested on:

- LXD, version 5.9

## Setup

- `cp discovery.conf /etc/zabbix/zabbix_agentd.d/`
- `import Template`

## Discovery rules

'sudo lxc ls volatile.last_state.power=RUNNING -f json' = Returns only Running containers
'sudo lxc ls -f json' = Returns All containers


## Contributions

If you find anything fishy or have a feature request, add a new issue and I'll take a look.

Pull requests appreciated.
