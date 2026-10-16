# Network Data

Source: ITPIE:OPS Documentation — Network Data
Source URL: https://itpie-hostname/documentation/content/features/network-data.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Network Data
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Summary
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] The Network Data feature lets you store user-provided network metadata that ITPIE cannot collect on its own (locations, customers, VLAN/VRF assignments, end-of-life records, etc.) and uses that data to enrich Search, Custom Reports, and Maps.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Network Data replaces the older Network Variable Data Management (NVDM) feature that was available in the Angular UI. The Blazor UI provides a fixed set of built-in entity tables (no user-defined entities or custom fields). Each table supports manual record entry, and most also support bulk CSV import; the Locations tab instead imports locations from a KML/KMZ file.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Built-in Entity Tables
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] The Network Data page is organized as a set of tabs. Each tab manages records for one of the built-in entities:
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Tab Purpose
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Locations User-defined sites, buildings, rooms, or geographic points used to tag devices on maps and in reports.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Customers Customer records used to associate devices, VLANs, and VRFs with a downstream tenant for impact reports.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] VLANs User-provided VLAN identity and description data.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] VRFs User-provided VRF identity and description data.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Networks Subnets/prefixes on your network with optional metadata (e.g., Infrastructure flag) used by Maps and reports.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Devices Devices manually entered when SSH/SNMP collection is not available; appear in Search, Custom Reports, and Maps.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] VLAN Mapping Maps a Customer to one or more VLANs on specific devices to drive the customer-impact report.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] VRF Mapping Maps a Customer to one or more VRFs on specific devices to drive the customer-impact report.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] End of Life Catalogs End-of-Product-Sale and End-of-Service-Life dates by vendor / product ID; feeds the EoPS / EoSL report.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Authorization
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Network Data implements the feature access permission scheme. Permissions are assigned per role on the Settings → User Management page.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] None: The user cannot see Network Data in the sidebar and cannot access the Network Data page if navigated to directly.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Read: The user can see Network Data in the sidebar and view records on every tab.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Write: The user can create, edit, import, and delete records on every tab.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Configure: No additional configure-level functions exist for Network Data; this level behaves the same as Write.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Working with Records
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Each tab presents a data grid with column-level filtering, sorting, and paging. For roles with Write access, a toolbar above the grid provides Add , Import CSV ( Upload KML/KMZ on the Locations tab), and Delete Selected actions.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Add a new record using an inline form that opens in place of the grid. Save the record, or use the Back to button — labeled with the current tab, e.g. Back to Customers — or Cancel to return to the grid without saving.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Edit or Delete a single record using the inline buttons in the row's Actions column.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Delete Selected removes records in bulk: check one or more rows using the selection checkboxes, then click Delete Selected in the toolbar.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Import CSV loads records in bulk from a CSV file. The import panel links to a downloadable CSV template for the entity.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] CSV Import Validation
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Each row in the CSV file is validated and imported independently. When the import completes, a results grid reports a per-row Success or Failure status with error details. Valid rows are saved even when other rows fail — correct the failed rows and import just those rows again.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Importing Locations from KML/KMZ
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] The Locations tab has no CSV import. Instead, the Upload KML/KMZ button opens a panel that imports geographical locations from a .kml or .kmz file. Locations whose names duplicate existing records are automatically suffixed to avoid conflicts.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Where Network Data Is Used
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Search — find impact|customer uses VLAN Mapping and VRF Mapping records to identify which customers are impacted by a device.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Custom Reports — built-in reports such as the EoPS / EoSL report use End of Life records as a join source.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Maps — Networks records flag certain subnets as Infrastructure (rendered with a pipe icon), and User-Provided Devices appear as map nodes with the UP glyph.
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Note
[ITPIE:OPS Documentation | Network Data | https://itpie-hostname/documentation/content/features/network-data.html] Custom entities, custom fields, calculable fields, indices, and folders from the legacy NVDM page are not part of the Blazor Network Data feature. If you previously relied on a custom entity, contact ITPIE support to discuss alternatives.