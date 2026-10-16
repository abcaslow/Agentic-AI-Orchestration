# 3.3.12 Release Notes

Source: ITPIE:OPS Documentation — 3.3.12 Release Notes
Source URL: https://itpie-hostname/documentation/content/release-notes/3.3.12.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] 3.3.12 Release Notes
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Infrastructure
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Upgraded to .NET 10 (SDK 10.0.201).
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Upgraded to Angular 20.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Upgraded to PostgreSQL 16.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Upgraded ReGraph to version 5.9.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Upgraded Npgsql to version 10.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Fixed a crash caused by PostgreSQL connection pool exhaustion.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Agents
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Remote agents now gracefully handle connection timeouts rather than crashing with an unhandled error.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Collection
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: Expanded the "Setup Site" wizard to support additional collector types beyond SSH.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: Added mode command support for SSH collection.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: Added a confirmation modal to the "Run Now" button to prevent accidental triggering.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: Added Collection and Export permissions to enable granular access control.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: The Generic API collector now supports offset and limit request headers.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: The GenericRestAPI collector output file now includes the collector type in its filename.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: Added IPv6 route support for Cisco ASAS, Arista EOS, and NX-OS.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] CHANGED: Renamed Cisco Viptela to Cisco SD-WAN in data sources and filters.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Fixed a constraint violation that could occur when deleting a job during an active collection.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Panorama collection no longer tracks and surfaces spurious device exceptions.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Made multiple stability improvements to the collection pipeline, including resource leak fixes, async/await correctness, and CancellationToken propagation.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Fixed null reference issues in the Cisco DNAC and Microsoft Graph collectors.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Running multiple collection jobs in succession no longer causes a deadlock.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: SNMP timeout settings now apply correctly.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: SNMP now reports a clear error message when the community string is incorrect.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Repaired collection diagnostics.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Invalid credential status now reports correctly.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: WMI collections on OPS no longer fail with a dependency injection error.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Fixed a null reference issue in the WMI collector.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Creating a collection file no longer crashes.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: The Export Sites option no longer appears enabled when no site exists.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: The collector type column now sorts correctly.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Improved collection times for large NX-OS switches.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Expanded Device Support
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Extended diagnostic coverage with reduced unknown values for the following platforms:
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Cisco : AP-COS (hostname, FQDN), CIMC (hostname), UCOS (system time), FMC, ADEOS, standard IOS (system time)
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Dell : FTOS manufacturer type and platform
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] VMware : ESXi (boot image file, manufacturer type), Photon OS
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NetScout PFOS : manufacturer type
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Aruba : ArubaOS system time
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Juniper SSR : hostname and FQDN
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Apple macOS : system time, hostname and FQDN
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Linux : system time
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] IronWare : system time
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] APC : system time format
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Various additional platform and manufacturer type unknowns resolved across multiple vendors
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Desktop Collector
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: The Desktop Collector interface now displays HTTP collection output.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: Added full command text editing with file rename support to the command catalog.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: The application now shows an improved error dialog when the sites configuration file is invalid or malformed.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: The Site Setup wizard now correctly creates new sites.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Fixed an error with AWS region configuration during cloud collections.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Fixed an issue with cloud endpoint ID handling.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Sort by Collector Type now works correctly.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Elapsed time now displays for failed collections.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: The application no longer becomes unresponsive when events arrive too quickly.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: The discovery configuration link now points to the correct page.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Run collection tooltips no longer cause spurious extra requests.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] CLI Collector
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: The CLI Collector now uses System.CommandLine for argument parsing, providing improved help output and validation.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Search
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: IP address array fields now support CIDR searches.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: Find Route now accepts IPv6 addresses as input.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: Migrated find device, find phone, find inventory, and configuration backup list to Query Endpoints for improved performance and stability when more than 10,000 rows returned.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Find Route now correctly displays IPv6 prefix notation and BGP values.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: The Find MAC typeahead now only suggests values that have corresponding MAC FDB entries.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: The "Clear" button on grid filters now correctly resets both the filter and the input text.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: find vlan * now returns results correctly.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: NetBIOS search now returns results correctly.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Fixed query errors in find mac functions.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: find virtualmachine no longer returns an error.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: find host * no longer throws an exception.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: find ActiveDirectory no longer returns a 500 error.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Resolved backups search issues.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Maps
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: Users can now save the Network View as a separate map from the Geo Map view.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: Geo Locations now display Map Stats-style data.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: Maps now render correctly at 1024×768 resolution.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: LAG relationships now register correctly without requiring a map reload.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Fixed an exception thrown during map snapshot.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: "Remove Selected" now saves the relationship between devices correctly.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: The Settings link in the map no longer navigates the user away to the Device Details drawer.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Annotations and Custom Boxes no longer disappear when using the "Show Only" context menu option.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: The Details drawer no longer appears blank for Annotations.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Proximity Cluster no longer prevents Unnamed Locations from displaying correctly in Geo Map view.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: "Add Missing Location Data" now works correctly.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Read-only users now see the appropriate context menu items.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: The device context menu now opens next to the selected device.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Expand/Collapse links now appear in the context menu.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Deleting a map folder no longer causes a console error.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: The application now redirects users to the maps index when the requested map does not exist.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Backups
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: Users can now select and download multiple backup files at once.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Backup config diff no longer incorrectly reports "1 line(s) different" when all lines differ.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Reports
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Exporting a report to CSV no longer includes hidden fields.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: The "NOT" operator in report conditions is now a toggle, not a dropdown.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Creating reports with certain Join conditions no longer produces an error.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: The "Reloading fields…" message now dismisses correctly after fields reload.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Multiple vertical scrollbars no longer appear in the report grid.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: The application now prompts users to save unsaved changes before navigating away.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Users can now drag report fields to the lower portion of the list when scrolled.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Device Details
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: Added a "Software" tab to the Device Details view.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Port status messages no longer hardcode the port number.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Port status messages now correctly reference the 65,535-byte limit.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] ZoneViz
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Creating a new world now correctly disables the starter enclave dropdown.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Users can no longer change the ZoneViz diagram type after creating the diagram.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Settings & Administration
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: Data Retention for configuration backups allows up to 5 years.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: Data Retention default for configuration backups is 1 year.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: The STIG banner no longer appears empty after updating settings without restarting the server.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Significantly improved User Management page load performance.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: OU filtering now applies correctly to the Cyber Terrain report.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Year fields now enforce a 4-digit limit.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] General UI
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: Corrected oversized confirmation modals and restored warning background colors.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] FIXED: The About dialog no longer expands to fill the entire screen.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Sidebar navigation labels are now lowercase for consistency.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Multi-sort index numbers no longer appear in Device Details grid column headers.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Updated the Backups sidebar icon to a history icon.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Known Issues
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] In some cases, values which should report as <unknown> report as <none> instead.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Maps: Geo-Map: Editing a device causes a 500 error in the console.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Coming Soon — Blazor
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] The following features are part of an ongoing update to the web application interface and will be available in a future release.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] General
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Users are able to configure their preferred grid page size, saving it as a personal preference across sessions.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] The application supports keyboard shortcuts for navigating and interacting with maps.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] The application displays page titles in the main header bar.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Improved navigation menu sizing and contrast.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Tooltips on action buttons throughout the application.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Infrastructure
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NEW: ITPIE Server will support Linux ARM64 ( linux-arm64 ) as a target platform.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Authentication & Authorization
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Authorization management will be available directly in the web application.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] The User Management page will include a toggle to hide disabled users.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Agents
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] The Agents management page will receive a significant UI refresh with improved layout and usability.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Collection
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] The Endpoints tab will become Collected IPs .
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] The Add to Target modal will support creating a new target without navigating away.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] The Jobs management page will receive a UI refresh with improved layout and status badges.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Grid views will support network-aware IP address filtering (e.g., searching by subnet returns all matching addresses in that range).
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Config Backups
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Config Backups filter selection labels will reflect clearer naming.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Discovery
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] The Discovery Management Summary will include All and Success summary cards.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Maps
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Users will be able to export maps to save and share map data.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Map initial load performance will improve.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Geographical map search will gain enhancements.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Maps will support more granular permissions.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] CHANGED: The map legend will move to the side panel.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Network Data
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] NVDM (Network Virtual Device Manager) will become Network Data throughout the application.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] The application will prevent editing or deletion of system-authored built-in VLAN and VRF entries.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Search
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Improved IP/CIDR filtering, column filters, and paging behavior.
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] Settings
[ITPIE:OPS Documentation | 3.3.12 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.12.html] The Presentation settings page will include a license management section.