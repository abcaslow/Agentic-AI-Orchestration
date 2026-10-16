# 3.3.10 Release Notes

Source: ITPIE:OPS Documentation — 3.3.10 Release Notes
Source URL: https://itpie-hostname/documentation/content/release-notes/3.3.10.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] 3.3.10 Release Notes
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] 🚨 Breaking Changes
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Desktop Collector
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Desktop Collector now only supports storing collection results in .zip format.
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] No action is needed - collections that previously used the Directory format will now automatically use the .zip format.
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Desktop Collector now requires a license feature ( AllowPlaintextCollectionFiles ) to produce decrypted collection results
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Action required: Any licenses that were previously issued do not have the AllowPlaintextCollectionFiles license feature - contact ITPIE customer support to have a new license created.
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] If the active license does not have the AllowPlaintextCollectionFiles license feature, you will be prompted to enter a password after running the collection. This password is used to encrypt the .zip file, and must be provided to decrypt the .zip file.
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] A default password can be specified via the Tools → Settings menu.
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] If the active license Desktop Collector has the AllowPlaintextCollectionFiles license feature, use the Tools → Log Decrypter menu to decrypt the files.
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Encrypted .zip files cannot be imported into OPS at this time.
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Collection (OPS)
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] The Verify Certificates option (when editing targets) has been fixed.
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Action required: All targets that use self-signed (or otherwise invalid) certificates must be verified to ensure the Verify Certificates checkbox is unchecked.
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Previous behavior: The Verify Certificates option always behaved as if the checkbox was unchecked, even if it appeared to be checked.
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Security
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Removed “Export as Excel” from the application
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Invalidated user’s session if their remote IP address changed
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Removed sensitive information from DSC files
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] General
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Retired legacy license key format
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] External Data Sources were updated, including ISO 3166 Country Codes and IEEE OUI MAC Address lookups
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Infrastructure
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Updated to Angular 18
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Updated to .NET & AspNetCore 8.0.17
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Changed application build timestamp to UTC
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Authentication & Authorization
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Replaced the limited emergency-account CLI with the comprehensive user-management CLI
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Default feature access levels and OUs can be setup to simplify access for new users
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Improved the login page
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Clarified the LDAP login form
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Differentiated external login buttons
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] NEW: security and performance assessments can be generated for devices from several pages in the application such as device details or configuration backups.
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] The AI Chatbot name is now configurable
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] You can now upload documents to the chatbot
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] SSH collection output is stored and accessible in AI chatbot
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Agents
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Agents now report the agent version to the application server
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Agents can now be archived
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Collection
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] NEW: Cisco ISE Live Log collection type and find log search for TACACS log now supported
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] NEW: Option to configure SSH commands per second and character delay
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Added failure count and failure % to jobs list
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Added links to jobs in target list
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Removed legacy log-decrypted file import
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Cisco 8500 Catalyst Router: support command show vrrs pathway
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Added support for OSC escape sequences
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Add show vrf detail command & parser for Cisco NX-OS
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Fixed fingerprinting issues found with Gigamon devices
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Expanded IPv6 support
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Desktop Collector
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] NEW: Option to auto-add discovered IPs after collection
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] NEW: The applied license can now be changed
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Decrypted zip files capability is now licensed
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Fixed issue that caused a crash when you run a collection with the ‘Trace Diagnostics’ option enabled
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Maps
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Geographical view mode has received several updates
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Devices can be directly added to a new unnamed location
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] You can navigate back and forth between network & geographic views
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] You can open the network view of a specific location on the geographic view
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] NEW: Added new layout features allowing aligning and distributing selected map nodes
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Reports
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] NEW: Discovery - Cyber Terrain report showing key services and their client information
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Added Send to Map feature
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Moved Built-in Reports to “Built In” folder
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Known Issues
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] In some cases, values which should be reported as are being reported as
[ITPIE:OPS Documentation | 3.3.10 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.10.html] Maps: Geo-Map: Editing a device cause 500 error in console