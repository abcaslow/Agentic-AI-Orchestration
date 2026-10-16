# Manual Export

Source: ITPIE:OPS Documentation — Manual Export
Source URL: https://itpie-hostname/documentation/content/features/manual-export.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] Manual Export
[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] Summary
[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] If your ITPIE instance is not able to access ServiceNow, you can still export your ITPIE data by following this manual procedure.
[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] First, you need to export your data from ITPIE. The easiest way to do this is to create a report based off of the search source that you want to import into ServiceNow. In the report, you can filter the results and select just the fields that you want to import into ServiceNow. Run your report, and export the data as a .csv file.
[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] Search for "import" in ServiceNow and select "IntegrationHub - Import."
[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] In the upper right, click on "Create new integration."
[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] Select a name and description. For Application, select CMDB Workspace (possibly not necessary).
[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] Select a source type of file, and choose CSV.
[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] Choose the file you want to import. The fields in the file will appear on the right.
[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] Select "Map to target" on the left.
[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] Add a table and choose the SourceNow table to import into.
[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] Search and enter the table you want.
[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] Select transform settings to map fields from your import into the ServiceNow table.
[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] Choose your transform settings. (It looks like you have to change something to enable the save button, but you can change it back.)
[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] Click on the more options menu and select "Edit mapping."
[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] Add fields one at a time, select the SourceNow field on the left and the import field on the right. "Match" indicates that the field will be used to determine if this is a new record or an update (corresponding to "Unique" in the ITPIE mapping system).
[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] When you're done, save your changes and select "Schedule imports" to run your import.
[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] You can schedule the import, or just click "Run Import" to execute.
[ITPIE:OPS Documentation | Manual Export | https://itpie-hostname/documentation/content/features/manual-export.html] When you make future imports, you will import new files, but you can keep the same transform.