# Collector agent

Source: ITPIE:OPS Documentation — Collector agent
Source URL: https://itpie-hostname/documentation/content/install/collector-agent.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Collector agent
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] The collector agent expands the capabilities of the application server by allowing collection jobs to run on a separate server elsewhere in your network.
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Requirements
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Collector agents may be installed on physical or virtual servers running Enterprise Linux or Windows Server.
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Managed Devices CPU Memory Storage
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] 0-2000 2 cores 8 GB 50 GB
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] 2000-5000 4 cores 16 GB 50 GB
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] 5000+ 8+ cores 32+ GB 50 GB
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Installation
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Linux
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Windows Server
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Install the RPM package. dnf will automatically install required system dependencies ( libicu , libcap ):
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] sudo dnf install itpie-collector-agent-<version>.rpm
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] The installer places a default configuration at /etc/itpie-collector-agent/agent.conf (copied from the example at /usr/share/itpie-collector-agent/examples/agent.conf ) if one does not already exist.
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Review and edit the configuration file before starting the service:
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] vi /etc/itpie-collector-agent/agent.conf
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Enable and start the service:
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] systemctl enable --now itpie-collector-agent
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Unzip the package to a user controlled location, which will become the working directory of the service. For example:
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] C:\ITPIE Collector Agent
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Copy or rename an example configuration to agent.conf in the working directory. Edit it before starting the service, although configuration should be reloaded automatically and reapplied when required by the agent.
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Run the installation script to create the service: "ITPIE:OPS Collector Service".
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] .\InstallService.cmd
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] You should configure the Windows service before starting it, depending on your organizational requirements (startup type, environment, recovery options, etc.).
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] When the service starts, it should create the necessary application directories:
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] C:\ProgramData\ITPIE\ITPIE Collector Agent
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Check the Application logs in the Windows Event Viewer for success.
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Configuration
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] In the configuration file for a collector agent, the following properties can be specified:
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] ServerUri : The address of the application server
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Default value: https://localhost
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] VerifyCertificates : Specifies if SSL/TLS certificates should be verified
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Default value: false
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] ConcurrentRequests : Specifies the maximum number of endpoints the collector agent will attempt to connect to simultaneously.
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Default value: 40
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Minimum value: 1
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Maximum value: 100
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] The agent must be restarted before changes to these settings will take effect.
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Note
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Variability of concurrent request limit
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] When using collection agents, due to variances in response times over the network, it is possible for the number of concurrent endpoints to be slightly higher than the configured limit. The number of concurrent endpoints will never exceed 110% (rounded down) of the configured limit.
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] For example, if the configured limit is 55, there will never be more than 60 concurrent endpoints.
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Note
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Performance impacts of changing concurrent request limit
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Initially, it may seem that raising the maximum number of endpoints from 40 to 80 would halve the time it takes to complete a job. This may not be the case, however, since each connection has overhead. It is possible that increasing the maximum number of endpoints can increase the time it takes to complete a job.
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] The impact of changing this value depends on many external factors. If the maximum number of concurrent endpoints is changed, the agent should be monitored to identify any performance impact. If a significant performance impact is identified, the change should be reverted.
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] Example configuration file
[ITPIE:OPS Documentation | Collector agent | https://itpie-hostname/documentation/content/install/collector-agent.html] { "CollectorAgentOptions": { "ServerUri": "https://itpie.example.com", "VerifyCertificates": true, "ConcurrentRequests": 20 } }