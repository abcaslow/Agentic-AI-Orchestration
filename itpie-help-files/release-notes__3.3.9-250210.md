# 3.3.9-250210 Release Notes

Source: ITPIE:OPS Documentation — 3.3.9-250210 Release Notes
Source URL: https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] 3.3.9-250210 Release Notes
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] General
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Achieved certification on the DoDIN Approved Product List (APL): TN 2401001; VAE ITPIE 3.3.9
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] All private keys for code signing certificates are stored on hardware certified as FIPS 140 Level 2, Common Criteria EAL 4+, or equivalent.
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] External Data Sources were updated, including ISO 3166 Country Codes and IEEE OUI MAC Address lookups
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Bug fixes and performance improvements
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Framework and library updates for performance and improved security including .NET 8 and Angular 17
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Web server now supports TLS 1.3
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Database now supports new versions of PostgreSQL 14, 15, and 16; and we have dropped support for PostgreSQL 11 and 12.
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Numerous query optimizations and additional logging during Network Analysis
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Analysis Optimization
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Device
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Network Relations
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] NEW: Remote Agents
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] ITPIE now supports running collections in a separate agent process that can be deployed in restricted network environments. With this capability, you can now collect network devices that behind firewalls and significantly speed up large collections by horizontally scaling out the number of agents that perform collections.
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] These agents can also be used to distribute and scale up AI/ML workloads.
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] New server-side auditable events include agent announcement, de/authorization, and connections. New client-side (agent) auditable events include the usual application lifetime events (start up and shut down), identifier reads and writes, remote authorizations, and service connections.
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Relevant install and admin documentation is provided in the user guide.
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] NEW: ITPIE ChatBot
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] We added support for running an internal ITPIE chatbot backed by an LLM trained on the ITPIE documentation. This goes hand in hand with Machine Learning Agents that are required to process AI/ML requests.
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] In the future, the ITPIE chatbot will be trained on raw collection output, user provided documentation, and the analyzed results from ITPIE collections, providing a natural language interface to all the ITPIE data.
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Collection
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] NEW: Advanced Collection Options for SSH Targets to ensure greater device compatibility
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Commands per Second: the maximum number of commands we emit per second when collecting on the endpoint
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Inter Character Delay: the time between each character sent as we run commands against the endpoint
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] NEW: Remote Collection Agents
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Remote collection agents can be used to collect on devices that are behind stateful firewalls that ITPIE cannot directly access
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Remote collection agents can distribute the collection process across multiple servers. This significantly reduces collection time and makes collections more robust to transient failures.
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Remote collection agents are supported on Linux and Windows providing an additional way to collect on WMI devices. Limited MacOS support is also available.
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Organize Agents and Jobs into “Sites”
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Each collection job can be assigned to a “site”
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Each remote collection agent can be assigned to a “site”, all of the remote collection agents assigned to the site will be available to collect on the devices in that collection job
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] NEW: Generic API Collector:
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Adds a customizable collector type that works for many different HTTP APIs
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Works for a broad range of HTTP APIs
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] ITPIE Resident Engineers can add support for additional APIs without needing to upgrade ITPIE
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Contact your ITPIE resident engineer or ITPIE support if you would like to add support for additional APIs
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] NEW: Expanded Collection Support of several new devices and element managers including
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Cisco Catalyst SD-WAN Manager
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Cisco Firepower Thread Defense (FTD)
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Cisco Nexus Dashboard Fabric Controller (NDFC)
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Cisco Secure Firewall Management Center (FMC)
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Dell iDRAC
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Dell OpenManage Enterprise (OME)
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Gigamon Fabric Manager
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] OpenGear Lighthouse Element Manger
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Bug Fixes
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Add support for swapping out devices with the same management IP
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Maps
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] NEW: Added a new Geographic Map View Option
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] You can add generic locations which can be configured to include points and polygons with names for easy reference.
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] You can import a set of points or polygons by uploading KML / KMZ files.
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] This includes tile server settings which you can use to customize the map tiles that are rendered as the background of your maps (see the user documentation in the Settings | Configuration section).
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] NEW: IPv6 Support was added in the Network Filter
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] NEW: Logical L3
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Custom nodes can now be added to the Logical L3 map
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Updates were made to the Logical L3 details drawer
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Includes support for Snapshots, Search and Filter
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] NEW: Multiple snapshots can now be added for any map
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] NEW: You can now compare two different maps and show differences between snapshots of the same map.
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Custom Reports
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] NEW: VLAN Utilization Report
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] NEW: IP Forwarding Rollup Report
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Bug Fixes
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Fixed column sorting issue in exported .csv
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Fixed populating First Seen and Last Seen in VLAN report
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Fixed VRF Counts not to require /32 when specifying
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] NVDM
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] NEW: Added a more complete “User Provided Devices” feature which can be used to add detailed entries for devices that are not collected on by the system but tracked by the user.
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] These devices can appear along collected devices throughout the system in search, maps, and other areas in the app
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Over time, this functionality will allow for the same details provided by our collected analysis.
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Zone Viz
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] NEW: Added a new “Simplified View” which presents a cleaner visualization of the security stack
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Settings
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Removed the “Use new analysis” option since the newest analysis technology has fully replaced the previous version
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Bug Fixes
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Fixed an issue that prevented importing user lists
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Known Issues
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] All of these issues are scheduled to be resolved in the next hotfix release
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Some map links are not displaying for certain systems (Dell iDrac, Cisco Nexus 9k, Cisco 8000v and Palo Alto)
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] User Provided Devices: issues with integration in maps user interface
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Custom Reports: extra fields are being included in exports
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Search: find device returning duplicate rows for Junos devices
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] Search: some column filters don't display all possible options to filter on
[ITPIE:OPS Documentation | 3.3.9-250210 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.9-250210.html] User Management: in some cases, newly created users have less permissions than expected