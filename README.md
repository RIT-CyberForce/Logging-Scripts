# Logging Scripts

This repository contains files necessary to set up logging, import custom configs, import custom rules, etc.

Current Focus: Wazuh

`local_rules.xml` - A collection of rules developed for Wazuh. Currently only contains rules for Windows systems. 

note: after running auditd rules, reload and verify that the rules are in place:
  # auditctl -R /etc/audit/rules.d/audit.rules
  # auditctl -l

note: after implementing wazuh configs, restart wazuh-agent/wazuh-manager depending on role
