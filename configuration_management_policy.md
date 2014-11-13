# Configuration Management Policy

Zane Benefits standardizes and automates configuration management through the use of Ansible as well as documentation of all changes to production systems and networks. Ansible automatically configures all Zane Benefits systems according to established and tested policies, and is used as part of our Disaster Recovery plan and process.

## Applicable Standards from the HITRUST Common Security Framework

* 06 - Configuration Management

## Applicable Standards from the HIPAA Security Rule

* 164.310(a)(2)(iii) Access Control & Validation Procedures

## Configuration Management

1. Ansible is used to standardize and automate configuration management.
1. No systems are deployed into Zane Benefits environments without approval of the Zane Benefits CTO.
1. All changes to production systems, network devices, and firewalls are approved by the Zane Benefits CTO before they are implemented.
1. An up-to-date inventory of systems is maintained using Google spreadsheets and architecture diagrams hosted on Google Apps and Drive. All systems are categorized as production and utility to differentiate based on criticality.
1. Clocks are synchronized across all systems using NTP. Modifying time data on systems is restricted.
1. All front end functionality (developer dashboards and portals) is separated from backend (database and app servers) systems by being deployed on separate servers.
1. All software and systems are tested using unit tests and end to end tests.
1. All committed code is reviewed using pull requests (on Github) to assure software code quality and proactively detect potential security issues in development.
1. Zane Benefits utilizes development and staging environments that mirror production to assure proper function.
1. Zane Benefits also deploys environments locally using Vagrant to assure functionality before moving to staging or production.
1. All formal change requests require unique ID and authentication.
