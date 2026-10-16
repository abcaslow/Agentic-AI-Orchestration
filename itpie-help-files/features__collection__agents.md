# Agents

Source: ITPIE:OPS Documentation — Agents
Source URL: https://itpie-hostname/documentation/content/features/collection/agents.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Agents
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] ITPIE supports the use of agents to assist it with Collection and AI/ML processing. These agents are services that can run on Linux, Mac, or Windows. Agents allow ITPIE to scale up collection, navigate stateful firewalls, and process AI/ML workloads on hardware suited to the task without impacting the ITPIE OPS server itself.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Installation and Administration
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] See the installation instructions for the agents here:
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] ITPIE Collector Agent
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Remote Agents Administration
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Viewing agents
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] To view the available agents, click the Collection icon on the left, then click on Agents link in the top navigation bar.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Agent List
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Name Description
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Agent Name The name of the Agent
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Agent Type The type of agent: MachineLearning or Collection
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Platform The platform: Linux , Windows , OSX
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Site Name A customizable value indicating which site this agent belongs to
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Connection Status Indicates if the Agent is currently connected: Connected or Disconnected
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] IP Address IP Address of the agent (often in IPv6)
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Is Authorized Indicates if the agent has been authorized by a super user: true or false
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Authorized By The email address of the super user who authorized the agent
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Authorized At The date and time when the agent was authorized by a super user
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Last Activity At The date and time when some message was last observed on the agent
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Created At The date and time the agent registered itself with ITPIE
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Modified At The date and time when the agent record was last modified
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Modified By The user who last modified the agent record
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Action The available actions for the agent: Edit , Authorize , and/or Deauthorize
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Each agent has two properties that can be configured, by clicking the Edit button for that agent.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Agent Name
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] The agent name is a customizable value that can be used to give the agent a descriptive and meaningful name.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] The default agent name consists of the agent type, a number, the agent's platform, and a unique identifier.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] ITPIE does not rely on this name; you are free to change it to any value that suits you.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] This value must be unique across all agents.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Site Name
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] By default, agents have a site name of Default Site .
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] The agent site name is used to group a set of agents together into a site .
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] The name Internal (case insensitive) is reserved for use for ITPIE, and cannot be used.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] The site name is only used by Collection agents; it is ignored by Machine Learning agents.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Authorizing an Agent
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Upon startup, an agent will connect to the ITPIE server specified in its configuration file (see Remote Agents Administration ). After the agent connects to ITPIE for the first time, a super user must authorize the agent before it will be used for any work.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] A super user can authorize an agent by clicking the Authorize button for that agent. After confirming with the dialog that is shown, the agent will be authorized.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] After authorization, the Is Authorized column in the table will change to true for that agent, and the Authorize button will change to a Deauthorize button.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Collection Agents Use Cases
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Use Case: Scalability
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Collection agents can be used to increase the scalability of ITPIE. The ITPIE server will collect on up to 40 endpoints at one time (this is not configurable). By default, collection agents will collect on up to 40 endpoints at one time, and this limit can be configured.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] By using collection agents, you can collect on a large number of endpoints at the same time. For example, if five collection agents are used, and each of those agents is configured to collect on 100 endpoints at a time, then up to 500 endpoints could be collected on simultaneously.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Use Case: Stateful firewalls
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Your network may have stateful firewalls that would ordinarily prevent ITPIE from connecting directly to your network devices via SSH or other network management protocols.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Instead of requiring you to add a firewall exemption to each of your managed network devices, collection agents establish two-way communication with the ITPIE server using HTTPS. Once two-way communication is established, collection can proceed. The collection agent will communicate with the network devices and then send the results back to the ITPIE server.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Use Case: FIPS mode and legacy devices
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] High security environments can enable FIPS mode on the ITPIE server's operating system. This will prevent ITPIE from using older encryption/hashing algorithms such as MD5 and DES. However, many of these organizations have legacy devices which do not support algorithms that are compatible with FIPS mode.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] A collection agent can be installed on a computer that does not have FIPS mode enabled on the operating system. This collection agent can then communicate with the devices that are not FIPS compliant, and the results are sent to the ITPIE server (over HTTPS, which is FIPS compliant) for processing.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] In environments that utilize FIPS mode, it is recommended to put collection agents that do not have FIPS enabled into a separate site from the collection agents that do have FIPS enabled.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Use Case: WMI (Windows Management Instrumentation)
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] WMI (Windows Management Instrumentation) is a Microsoft proprietary programmatic interface for the Windows operating system. ITPIE can use WMI to collect information about Windows computers (to include servers, desktops, and laptops). Unfortunately, since WMI is only available on Windows, the ITPIE server (which runs on Linux) cannot natively use WMI.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] If the ITPIE collection agent software is installed on a Windows computer, the ITPIE server can use that collection agent to collect data via WMI.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Sites
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] When ITPIE runs a job, it must first select one or more agents to run the job. A super user can group agents together into "sites" by configuring the agent's site name. Every agent with the same site name is considered to be in the same site.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] By default, all agents are in the site named Default Site .
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] The most common reason to use multiple sites is the existence of stateful firewalls in-between the ITPIE server and the other network devices.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] For example:
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] One or more collection agents are deployed within a firewall's internal network.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Each of those agents are configured with the same site name .
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Collection jobs contain only devices that are inside of that firewall's internal network, and are configured to use only agents from that site .
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] When the job is run, only agents from that site (which are behind the firewall) will be used for collection
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Note
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Agent Site Applicability
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] The machine learning agent does not support sites. Any site names that are specified for machine learning agents are ignored.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Changing an Agent's Site
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] To edit an agent's site name, click on the Edit button for the agent, and set the site name in the drawer.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Note
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Site Name Casing
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Agent site names are case insensitive. For example, Datacenter is considered to be the same as datacenter . To reduce confusion, it is recommended to use a consistent naming convention for site names.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Note
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Prohibited Site Names
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] The site name of Internal is prohibited. This restriction is case insensitive - for example, internal and InTeRnAl are also prohibited.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] Changing a Job's Site
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] When configuring a collection job , an agent site can be selected.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] The Internal agent site represents the ITPIE server itself. Jobs assigned to the Internal agent site will not use any collection agents that have been authorized; the ITPIE server will directly connect to the endpoints.
[ITPIE:OPS Documentation | Agents | https://itpie-hostname/documentation/content/features/collection/agents.html] If an agent site other than Internal is selected, then only agents that have that site name will be used for the job. Individual requests for that job will be distributed fairly between the agents in that site.