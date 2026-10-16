# IT Automation: A Case with Redhat's (now IBM's) Ansible — United with Code (Blog)

**Source:** https://smartnewdeal.com/it-automation-a-case-with-redhats-now-ibms-ansible/
**Author:** Bernie Wolzak | August 22, 2019 | Category: Technology
**Captured:** 2026-07-08

In this blog post, we review how an entire IT infrastructure — computing, storage and networking resources — can be automated using the tools Ansible and Terraform. Emphasis is placed on Ansible.

Ansible's tag line is that it delivers *Radically simple IT Automation*. It delivers on this through its playbook architecture supported by files such as inventory files that contain target device IP addresses and device credentials. Ansible was acquired by Redhat in October 2015. IBM purchased Redhat for $34 billion in July 2019.

An Ansible playbook example uses: (1) a playbook task section, (2) a specific Ansible task module called `ios_command` for running Cisco IOS CLI commands, and (3) a specific Cisco IOS CLI command to run. Once built, the playbook can be run on multiple devices by adding more IP addresses and credentials in the Ansible inventory file.

Sample Ansible inventory file:
```
[all:vars]
username=admin
password=admin

[ios]
192.168.58.124
192.168.58.130
172.16.0.66
```

**The Nuts and Bolts of Ansible: Python and Github.** Ansible is written in Python and is 100% open source, so you can explore its internals and modify the code. Ansible source is on GitHub (https://github.com/ansible/ansible); you can `git clone` the repo and keep it current with `git pull`. (Microsoft purchased GitHub for $7.5 billion in 2018.)

Both Microsoft and IBM made these acquisitions to counter Google and, more significantly, Amazon Web Services. Ansible playbooks can be deployed in AWS, Microsoft Azure and Google Cloud Platform.

**Trade-Offs:** Ansible is simple, and this simplicity can affect its capabilities and flexibility. Other tools are more powerful and flexible but more complex. (Reference: XebiaLabs Periodic Table of DevOps Tools.)

*Comment: Lania Caslow (June 2, 2020) — "Very interested, would like to learn more!!"*

*Unite with Code! © 2026 UnitedwithCode, LLC. All Rights Reserved.*
