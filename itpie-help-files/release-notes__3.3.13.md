# 3.3.13 Release Notes

Source: ITPIE:OPS Documentation — 3.3.13 Release Notes
Source URL: https://itpie-hostname/documentation/content/release-notes/3.3.13.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] 3.3.13 Release Notes
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] Infrastructure
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] CHANGED: Removed the legacy Angular web client. The Blazor UI is now the sole web interface and is served directly at the root path. Previous /ui/* paths now return 404.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] CHANGED: Removed the "Use Legacy UI" toggle from Settings → Preferences along with the associated user preference.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] NEW: Added a configurable migration command timeout ( MigrationCommandTimeout in itpie.conf ) so large schema migrations on tables like ans.net_macfdb no longer fail at the previous hard-coded 30 minute limit.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: Large live collections no longer cause the Blazor UI to briefly display a "Connecting" reconnect modal.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: SSH collection secondary analysis no longer fails with a "net_ifinfrastructure_entry" is not partitioned error.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] Security & Authentication
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: External identity provider login (Keycloak / OIDC) works end-to-end again.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: Unauthenticated users navigating to any Blazor page ( /search , /collection , /discovery , /network-data , /reports/custom , /settings , etc.) are now redirected to /login with a returnUrl instead of falling through to a NotAuthorized fallback.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] Collection
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] NEW: Added an Import Files button to the Collection Jobs page for users with Collection Configure permission, matching the prior Angular functionality.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] NEW: The aggregation status table now includes the endpoint / IP for each item.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] NEW: Added device support for HPE iLO firmware boot image; improved VOMV identification for CentOS Linux Stream.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] NEW: Added scrolling to the Add Site, Add Target, Add Target Folder, Add Credential, Add Job, and Add Job Folder dialogs so users with the browser zoomed in can reach the Save button.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] NEW: Added Interface Statistics collection and reporting.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: Saving an SNMP credential with version "V2c" no longer fails.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: The OU dropdown now shows only the assigned OU for non-superusers, and Collection Create / Update / Delete actions are hidden for read and write users.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: Saving a VRF Mapping or VLAN Mapping form no longer throws an error.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] Search
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: find arp <IP> no longer throws an error and crashes the page. Bare IPs are now accepted for ARP, Edge, Infoblox, Network, and VRF searches.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: find device <CIDR> and its detail view no longer error when the CIDR contains host bits.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: find route syntax handling corrected.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: find infoblox <mac> supports IPv6 MAC address syntax and no longer crashes the page.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: A runtime exception in the search grid column definition was resolved.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: Device IP columns in search results now link to Device Details consistently.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: Column sorting and filtering now work in the search results grid.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] Reports
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] NEW: Custom Reports are now available in the Blazor UI with a tabbed layout matching the rest of the app.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: The Reload Fields button is now disabled until the report is complete, preventing spurious clicks.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: Editing report indices now correctly resets the report results.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: Selecting Reload Fields on an empty report no longer displays an error.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: Missing navigation tabs inside Reports are restored.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: The UCPIE and Diagnostics report selectors now announce only the report title to screen readers.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] Network Data (formerly NVDM)
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: The Customers, VLANs, and VRFs form inputs no longer lose focus on Tab or keystrokes.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: The Locations Edit form now repopulates the Coordinates textarea.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: The OU Subnet form now uses a semantic Radzen TextArea, eliminating the nested input box.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: The Help link on Network Data pages now opens the correct feature documentation.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: Navigating to /network-data (with no tab segment) now renders the Locations grid instead of a "page not yet available" placeholder.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] Device Details
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] NEW: On macOS, the command field now supports a hand-mode toggle for copy/paste-friendly interaction.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: The uncollected IP table on Device Details now includes links back to Device Details for each device.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] Maps
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] NEW: Added Custom Shapes support, allowing users to place and style custom shapes on maps.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] ZoneViz
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: Diagram labels no longer render twice on expanded enclaves, network objects, and security zones in both detailed and simplified layouts.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] General UI
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: Menu contrast issues in light mode were corrected.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] FIXED: The page body scrollbar now appears only when needed.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] Known Issues
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] In some cases, values which should report as <unknown> report as <none> instead.
[ITPIE:OPS Documentation | 3.3.13 Release Notes | https://itpie-hostname/documentation/content/release-notes/3.3.13.html] Maps: Geo-Map: Editing a device causes a 500 error in the console.