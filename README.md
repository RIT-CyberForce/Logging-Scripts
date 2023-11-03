# Logging Scripts

This repository contains files necessary to set up logging, import custom configs, import custom rules, etc.

Current Focus: Wazuh

`windows_rules.xml` - A collection of rules developed for Wazuh Windows agents. 
`linux_rules.xml` - A collection of rules developed for Wazuh Linux agents.
`audit.rules` - rules for auditd
`main.sh` - **in progress** script to automate wazuh manager setup

note: after running auditd rules, reload and verify that the rules are in place:
  auditctl -R /etc/audit/rules.d/audit.rules
  auditctl -l

note: after implementing wazuh configs, restart wazuh-agent/wazuh-manager depending on role
