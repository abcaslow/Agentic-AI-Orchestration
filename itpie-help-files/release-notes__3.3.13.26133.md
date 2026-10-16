# 3.3.13.26133 Release Notes

Source: ITPIE:OPS Documentation — 3.3.13.26133 Release Notes
Source URL: https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] 3.3.13.26133 Release Notes
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] Discovery
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] NEW: Added an All IPs page under Discovery showing every discovered IP with a side-by-side detail pane covering Device Detail, Analyzed Entries, Discovery Protocol, ARP, MAC, Virtual Machines, DNS, Intune, Active Directory, Cisco ISE, Infoblox, Tenable, and Aruba ClearPass.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] Search
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] NEW: The Search page now supports query string parameters, enabling bookmarking and deep-linking of search queries.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] NEW: CSV export is now available via the right-click context menu on Search results, with full dark theme support.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] FIXED: Search navigation now hides areas for unlicensed features.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] Collection
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] NEW: Collection history is now displayed even when a collection has failed, so you can review what occurred.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] FIXED: A bug in the Generic API CLI collector has been resolved.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] FIXED: The ans_temp partition create/drop timeout has been raised to 30 minutes, preventing failures on busy servers with concurrent collections.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] FIXED: AWS collection no longer crashes when the AWS SDK returns a null item collection.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] Maps
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] NEW: Map tile server settings now include a test button that makes an HTTP request to validate the configured URI.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] CHANGED: Creating a new map now redirects immediately to the map editor.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] FIXED: "Select All" in the Add Node dialog now only selects devices that match the active filter.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] FIXED: The map detail information panel no longer displays duplicate entries.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] FIXED: Navigating away from and back to a map no longer leaves side panels in a stale open state.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] FIXED: Leaflet map CSS now loads correctly in Docker deployments, restoring proper map tile styling.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] Network Data
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] FIXED: Platform, Location, and System Location fields on Network Data Devices are now properly saved when creating or editing a device.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] FIXED: VRF and VLAN mapping forms no longer have re-rendering issues; missing values now display as <none> .
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] FIXED: The Help link on Network Data pages now opens the correct documentation.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] Reports
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] NEW: UCPIE report tables now support column sorting and filtering.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] Device Details
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] NEW: Backup Config single-device comparison now includes Previous/Next diff navigation buttons for stepping through timestamp comparisons.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] NEW: find config match results now deep-link directly to the matching line in Command Output, with the line highlighted in the editor.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] CHANGED: The command output navigation list is now flattened for easier browsing.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] FIXED: Device Details → Command Output no longer freezes when a device has the same aggregation ID across multiple logical systems.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] FIXED: Command output navigation buttons now correctly select the corresponding logical system.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] General UI
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] NEW: Tables throughout the application now support CSV export via right-click context menu.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] NEW: Job and Target folder views now support CSV export via right-click context menu.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] NEW: Folders in the Jobs and Targets tables can now be edited and renamed.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] FIXED: Deleting a folder in Jobs or Targets now immediately refreshes the item list without requiring a full page reload.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] FIXED: Unauthorized users are now correctly redirected when attempting drag-and-drop operations on Jobs, Targets, and Reports.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] Device Support
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] NEW: Added SNMP engine ID fingerprint support for Cisco ASA.
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] Known Issues
[ITPIE:OPS Documentation | 3.3.13.26133 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.26133.html] In some cases, values which should report as <unknown> report as <none> instead.