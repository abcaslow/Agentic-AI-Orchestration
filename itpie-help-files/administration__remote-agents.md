# Remote Agents

Source: ITPIE:OPS Documentation — Remote Agents
Source URL: https://itpie-hostname/documentation/content/administration/remote-agents.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Remote Agents
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Remote agents expand and enhance the capabilities of the application server by allowing certain workloads to run on a separate server elsewhere in your network.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] The current types of remote agent are:
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Collector agent
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Configuration
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] The agent's configuration file is written to a platform-specific location. Below are example paths, the actual paths will vary depending on the specific agent type and installation package implementation.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Linux
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Windows Server
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Includes the common package path and the service user's configuration path.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] /etc/itpie-example-agent/agent.conf /var/lib/itpie-example-agent/.local/share/itpie-example-agent/agent.conf
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Includes the common application data path and the current working directory.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] C:\ProgramData\ITPIE\ITPIE Example Agent\agent.conf C:\ITPIE Example Agent\agent.conf
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Agent options
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Common agent options include the following required keys:
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] ServerUri: The address of the application server. Defaults to https://localhost .
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] VerifyCertificates: If server certificates should be verified, true , otherwise false . Defaults to false .
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] The following is an example and the section name is generic. The section name will vary depending on the specific agent type and installation package implementation.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Collector Agent
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] "CollectorAgentOptions": { "ServerUri": "https://itpie.example.com", "VerifyCertificates": true }
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Logging
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] The logging section may contain multiple platform-specific subsections. The log levels for different categories can be fine tuned within each subsection.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Linux
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Windows Server
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] The "LogLevel" subsection controls journald messages.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] "Logging": { "LogLevel": { "Default": "Information", "Microsoft": "Warning", "Microsoft.Hosting.Lifetime": "Information" } }
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] The "EventLog" subsection controls Event Log messages.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] "Logging": { "EventLog": { "SourceName": "ITPIE.Example.Agent", "LogName": "Application", "LogLevel": { "Default": "Information", "Microsoft": "Warning", "Microsoft.Hosting.Lifetime": "Information" } } }
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Authentication and Authorization
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] An agent's identity is protected by a randomly generated identifier, created the first time the agent service is started, and written to a protected filesystem location. Below are example paths, the actual paths will vary depending on the specific agent type and installation package implementation.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Linux
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Windows Server
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] /var/lib/itpie-example-agent/.local/share/itpie-example-agent/identifier
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] ``` C:\ProgramData\ITPIE\ITPIE Example Agent\identifier ```
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] The agent sends its identifier, and other important metadata, to the application server, via an HTTP REST API call, as an "announcement" that the agent exists. The server responds with a temporary authorization token that the agent may use to confirm authorization and, once authorized, to receive work.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] The agent appears in the agents list on the application server and must be authorized by an application superuser. Once authorized, the agent may use the temporary authorization token or, if expired, request another, to open a WebSocket for the purposes of recieving and reporting on work.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Auditing
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Remote agents implement several categories of auditable events.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Event Categories
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Application Lifecycle
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Application lifecycle events are auditable. These are logged automatically by the Microsoft .NET Core hosting subsystem. We do not have control over these message tempates or event IDs. We reproduce them here completely for reference.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Example application started:
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] info: Microsoft.Hosting.Lifetime[0] Microsoft.Hosting.Lifetime: Information: Application started. Press Ctrl+C to shut down. info: Microsoft.Hosting.Lifetime[0] Microsoft.Hosting.Lifetime: Information: Hosting environment: Production info: Microsoft.Hosting.Lifetime[0] Microsoft.Hosting.Lifetime: Information: Content root path: /opt/itpie/itpie-collector-agent/
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Example application shut down:
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] info: Microsoft.Hosting.Lifetime[0] Microsoft.Hosting.Lifetime: Information: Application is shutting down...
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Authentication
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Reading and writing the identifier are auditable events.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] 1002: Read identifier.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Read identifier from '{PhysicalPath}': '{IdentifierHash}'
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] 1004: Write identifier.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Write identifier to '{PhysicalPath}': '{IdentifierHash}'
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Authorization
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Confirming authorization is an auditable event and should match a server-side generated event.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] 1100: Authorize agent.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Agent authorized at '{ServerUri}': '{IdentifierHash}'
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] External service connections
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] All external services connection attempts are auditable events. A configured host name should be resolved to one or more IP addresses, for the purposes of logging, although we cannot tell which IP address was resolved for the actual connection.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] 1500: Connect to external service.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Connect to external service: [{ServiceAddress}].
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] 1501: Connect to external service failed.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Connect to external service: [{ServiceAddress}]. FAILED: {Reason}
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] 1502: Connect to external service.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Connect to external service: {ServiceName} ([{ServiceAddresses}]).
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] 1503: Connect to external service failed.
[ITPIE:OPS Documentation | Remote Agents | https://itpie-hostname/documentation/content/administration/remote-agents.html] Connect to external service: {ServiceName} ([{ServiceAddresses}]). FAILED: {Reason}