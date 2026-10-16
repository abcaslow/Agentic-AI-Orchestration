# Machine-learning agent

Source: ITPIE:OPS Documentation — Machine-learning agent
Source URL: https://itpie-hostname/documentation/content/install/machine-learning-agent.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] Machine-learning agent
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] The machine-learning agent expands the capabilities of the application server by providing AI features.
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] Requirements
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] A machine-learning agent may be installed on a physical or virtual server running Enterprise Linux or Debian.
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] The minimum system requirements for the machine-learning agent are:
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] GPU CPU Memory Storage
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] 16 GB 4 cores 16 GB 200 GB
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] INFO
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] The minimum requirements are subject to change as capabilities are added to the machine-learning agent.
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] Installation
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] Linux
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] Install the package.
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] dpkg -i itpie-machine-learning-agent_*_amd64.deb
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] Install any missing depedencies:
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] apt-get install -f
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] Copy an example configuration to the system-wide location. Edit it before starting the service, although configuration should be reloaded automatically and reapplied when required by the agent.
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] install --mode 0640 --owner root --group itpie-machine-learning-agent /usr/share/itpie-machine-learning-agent/examples/agent.conf /etc/itpie-machine-learning-agent/agent.conf
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] Enable and start the service.
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] systemctl enable --now itpie-machine-learning-agent
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] Configuration
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] INFO
[ITPIE:OPS Documentation | Machine-learning agent | https://itpie-hostname/documentation/content/install/machine-learning-agent.html] See remote agents for more information on configuring a machine-learning agent. Note, the specific configuration subsection should be named "MachineLearningAgentOptions".