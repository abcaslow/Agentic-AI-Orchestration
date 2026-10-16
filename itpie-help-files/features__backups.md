# Config Backups

Source: ITPIE:OPS Documentation — Config Backups
Source URL: https://itpie-hostname/documentation/content/features/backups.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Config Backups
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Summary
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] The Backups feature provides Network Engineers with several capabillities including configuration file dowload, intra-device historical diff/compare, inter-device configuration diff/compare, etc...
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] The frequency that device configurations are downloaded, analyzed, and stored is managed via the Collections tab. Configuration has its own collection job type and is able to run more or less frequently than othr jobs types based on the operator's requirements. Optimally, Configuration collections should be scheduled separately from any other job type AND the job should be set to Skip Secondary Analysis . (See the Collection page for additional details)
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] As a best practice, configuration backups should be scheduled at least once a day. This provides a reasonable time frame to detect and audit changes while also allowing for outage restoral or configuration rollback when neccessary.
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Important
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Every device MUST successfully complete a Device level collection before running a Configuration-Only job.
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Getting Started
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Filter Dates
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] ITPIE filters backups by checking whether the first time the most recent backup version of a device falls within the specified date range (UTC Timezone).
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Time Filtering
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Operators can filter the list by using:
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Custom Start and End Date/Time selectors.
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Quick Range selections from the dropdown.
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Reset all filters to default with the Clear All button.
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Filtering on other criteria (columns)
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Example Scenario: Only specific backups
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Expand Width to see more columns (Click and drag the line to the right)
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Use the horizontal scroll bar to navigate to more columns
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Filter on the Columns
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Click on the three lines on the OS column then click on the symbol circled below
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Deselect all operating systems and check the desired operating system (example: Aruba)
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Filter on the Command Column as shown below (Example: “show config pushed shared template”)
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Backup File View
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Click on any device row to bring up the most recent configuration backup in the right panel.
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] View previously seen versions of the configuration from the Changed On drop down.
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] If there is a change history for the selected device, checking the Compare To box and selecting a different date will text compare the two backups and display the number of lines changed.
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] The selected backup can be downloaded with the Download Latest Device Log button.
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Device Configuration Comparison
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] In the event that two devices are intended to function as a redundant pair, such as Core Switches, FHRP Routers, or HA Firewalls, operators can compare the configurations of those two devices by:
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Select ONLY those two devices in the left side grid
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Click the "Compare Configuration" button in the right-hand window
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Since these are redundant core routers, we expect to see differences in an interface's specific IP Address. However, the router on the right having IP Address 10.110.10.12 is completely missing the interface Loopback 199 .
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Scrolling further down in the configurations reveals that router 2 is also missing an entire BGP EVPN EVI. Given a network in normal operating state, this error would not present itself. However, if a network failure does occur on router 1, router 2 would only resume -some- service.
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Finally we see router 2 is also missing the neccessary HSRP configuration for two interfaces. As in the previous example, these two networks would not fail over in the event that router 1 experiences a critical failure.
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Authorization
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Config Backups implements the feature access permission scheme.
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] None: The user cannot see Config Backups in the sidebar and the user cannot see the Config Backups page if navigated to directly.
[ITPIE:OPS Documentation | Config Backups | https://itpie-hostname/documentation/content/features/backups.html] Read: The user can see Config Backups in the sidebar and can access the Config Backups page. The user can view and download data for tabs in the Config Backups section.