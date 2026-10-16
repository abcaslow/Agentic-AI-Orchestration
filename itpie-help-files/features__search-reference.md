# Intelligent Search

Source: ITPIE:OPS Documentation — Intelligent Search
Source URL: https://itpie-hostname/documentation/content/features/search-reference.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Intelligent Search
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Command Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] INFO
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] About Command Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] We use a few conventions to describe the command syntax. Take the inventory command as an example:
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find inv[entory]|hard[ware] <ip|hostname|serial|productid|name|desc>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Aliases for subjects are separated by a pipe | . Any characters for a subject surrounded by brackets [] are considered optional and may be omitted. For example:
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find inv *
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Will return all the results for the find inventory command, even though you didn't type it out fully.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Predicate types are contained in angle brackets <> and separated by a pipe |
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] INFO
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Types and Search
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Many of the option types have specific ways you can search. For instance, VLAN IDs have special filters, and becuase they are a number, you can't use wildcards. Typically, any text based predicate will support the use of the wildcard * symbol. If the * isn't present, then the search will assume you mean equality and will perform an exact match.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] We note in the reference below which predicate types support wildcards, and which do not.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Shown below is a list of all the find commands and options that ITPIE supports with the Search function.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Predicate Types
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] ITPIE Recognizes 5 types of predicates (or search terms). Depending on the type of predicate, we apply the search term to an appropriate value in the data set.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Predicate Type Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] IP We recognize IP Addresses if the value is a valid IP with no other text in the string (e.g. 1.1.1.1 would be recognized, but 1.1.1 would not, and *1.1.1.1 would also not be recognized)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] CIDR A CIDR is a valid subnet in CIDR notation i.e. 1.1.1.1/24 with no other text in the string. Similar to the IP Address above, 1.1.1.1/2* would be classified as text, and 1.1.1.1 would be recognized as an IP.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Number Any set of digits without periods or other text. 1 or 1234 are valid numbers. 1.2 and 12* are not valid numbers.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] MAC We will identify text as a mac if it has any two pairs of valid hex separated by a colon : . 11:22 and ab:12 and 00:00:5E:00:53:FF are valid macs. 3i:33 is not.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Text If the value has a wildcard * or doesn't match to any of the above, then it is considered text.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Depending on the command and what predicates it supports, not all of the above types are used. In some cases, say if the command only supports <ip> and <hostname> then if the term is matched to an IP predicate type it will get applied to the IP column and everything else will get treated as Text .
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Command Reference
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Active Directory
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find act[ivedirectory]|ad <fqdn|age> aged
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <fqdn> Yes Text FQDN The Fully Qualified Domain Name of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <age> No Number Last AD Change The number of days (prior to today) that you want to view records from
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] aged If the aged option is used, active directory searches within a time window from now back the number of days provided
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] AD Server IP The management IP of the Active Directory Server
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Domain Name The domain name of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] FQDN The fully qualified domain name of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] DNS Host IP The IP of the host
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Vendor The the Vendor of the Operating System
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name The name of the operating system
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version The version of the operating system
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version Full The full name/version of the operating system
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] AD Description The AD description for the host
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Manufacturer Type The type of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Distinguished Name The full location of the device using DN format
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last AD Logon The date/time the computer last logged on to AD
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last AD Change The date/time AD last record a change on the computer record
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the AD Computer entries that have 'laptop' in their FQDN
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find ad *laptop*
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the AD Computer entries that have changed in the last 180 days
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find ad 180 aged
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] ARP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns the set of ARP entries from the most recent collection of devices within the last known good window (typically 7 days of the last successful collection). Find ARP history goes beyond the last known good window.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find arp <ip|network|mac> find arp <ip|network|mac> hist[ory]
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP ARP IP The IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR ARP IP A network expressed in CIDR notation
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <mac> Yes MAC or Text MAC A MAC address that matches the MAC field
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] history Includes all ARP entries seen 60 days from the last collection
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] ARP IP The IP address as seen by ARP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] MAC The MAC address associated to this IP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface The name of the interface the ARP entry was associated with
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VRF Name THe VRF configured on the interface with which the ARP entry is associated
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Network Prefix The subnet (Network Prefix) of the interface with the ARP entry
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Registration The OUI Registration for the vendor associated with the MAC address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OUI Country The vendor's country of origin based on the OUI Registration
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] MAC48 Type The MAC address type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Proxy ARP Whether the interface is running in a Proxy-ARP mode
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Seen From The date/time this record was first seen in this form
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Seen To The date/time this record was last seen in this form
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] ARP entries are dated with Seen From and Seen To fields that indicate the time frame the ARP entry was seen in.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all ARP entries for the IP Address 172.30.16.9
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find arp 172.30.16.9
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all ARP entries contained in the Network Prefix 172.30.16.0/24
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find arp 172.30.16.0/24
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all ARP entries for the MAC Address 00:00:5E:00:53:FF
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find arp 00:00:5E:00:53:FF
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all ARP entries within 60 days from the last collection for the IP Address 172.30.16.9
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find arp 172.30.16.9 history
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all ARP entries within 60 days from the last collection, contained in the Network Prefix 172.30.16.0/24
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find arp 172.30.16.0/24 history
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Config
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find config|cfg <term> find config|cfg <term> exclude <term>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <term> Yes Text Any keyword to search in config output (minimum 3 characters)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] exclude Any keyword to exclude (minimum 3 characters)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Matched Count Number of output lines found to contain the search term
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Matched Lines Text of the output lines containing the search term
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Logical System Name The system's uniquely identifiable name within the network
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Manufacturer Type The type of device (e.g. Firewall, Router, Switch, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor The name of the Vendor who makes this device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model The model of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name The name of the operating system (e.g. IOS, JUNOS, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version The version of the operating system
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Command Text The command which produced the matched config output lines
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Updated The date when the command output was last collected
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Tip
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Pro Tips!
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] You can use multiple <include> or <exclude> terms by wrapping them in quotations!
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] You can search for partial terms using TRAILING wildcards ( * ) ONLY!
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Terms do NOT need to be in order.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] ALL Include terms are matched in the returned results!
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] ANY Exclude term is matched to filter the returned results!
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find config "priv* 15 passw*" exclude "encrypt* pbkdf2"
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all config output with lines that contain the word username
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find config username
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all config output with lines that contain the word username , but NOT the word admin
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find config username exclude admin
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Customer Impact
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Using data entered on the Network Data page that links VRFs and VLANs to specific customers on devices, you can use this command to find which customers are impacted by a change to a device.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find imp[act]|cust[omer] <ip|network|hostname>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Device IP The management IP of a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR Device IP A network address in CIDR notation that includes the management IP of a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <hostname> Yes Text, MAC, Number Hostname The hostname of a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Customer Name The name of the customer linked to the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Customer POC Point of Contact information for the linked customer
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] ID ID of the linked Customer configured on the Network Data page
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Type The type of link used: VRF or VLAN
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the customers linked to a VLAN or VRF configured on that device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find impact 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find de[vice]|dvc <hostname|ip|network> find de[vice]|dvc <hostname|ip|network> all find de[vice]|dvc <hostname|ip|network> det[ail]
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Status Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR Device IP A network expressed in CIDR notation (e.g. 192.168.0.0/23 )
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <hostname> Yes Text, Number, Mac Hostname The hostname or partial hostname of a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] all Results include devices from discovery sources that have not been directly interrogated
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] detail Results include additional columns related to protocol support
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] status Includes additional results specific to PING, SSH, and Telnet
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Logical System Name The name of the logical system configured on this device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Manufacturer Type The type of device (e.g. Firewall, Router, Switch, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor The name of the Vendor who makes this device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Platform The platform of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model The model of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Status The last collection status of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name The name of the operating system (e.g. IOS, JUNOS, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version The version of the operating system
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Copper Port Count The number of physical ports with a Copper cable type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Fiber Port Count The number of physical ports with a Fiber cable type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Unknown Port Count The number of physical ports with an cable type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Physical Port Count The number of physical ports
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Logical Port Count The number of logical ports
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] System Up Time How long the device as been running since the last reboot
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Boot Image File The image file the device boot from
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Domain Name The Domain Name configured on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] System Contact The SNMP System Contact
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] System Location The SNMP System Location
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] System Time The time from the perspective of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Protocols A list of the known operational protocols on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Discovery Source What source this information came from: Analyzed, CDP, LLDP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen When data for this record was last seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Seen When data for this record was first seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] SSH Status (Detail Only) If SSH (port 22) is currently enabled and running on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] PING Status (Detail Only) If the device responds to PING
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] PING Roundtrip (ms) (Detail Only) If successful, the roundtrip time in milliseconds for the PING
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Telnet Status (Detail Only) If Telnet (port 23) is currently enabled and running on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] CPU Utilization (Detail Only) The utilization of the CPU at the time of the last collection
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Memory Usage (Detail Only) The usage of the Memory at the time of the last collection
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] CDP (Detail Only) Is CDP running on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] CDP Count (Detail Only) Number of CDP neighbors on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] LLDP (Detail Only) Is LLDP running on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] LLDP Count (Detail Only) Number of LLDP neighbors on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] MSTP (Detail Only) Is MSTP running on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] RPVST (Detail Only) Is RPVST running on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] MPLS (Detail Only) Is MPLS running on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OSPF (Detail Only) Is OSPF running on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] ISIS (Detail Only) Is ISIS running on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] BGP (Detail Only) Is BGP running on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] L1 Protocols (Detail Only) If one of the following protocols is enabled on the device: ISDN, FDDI, Frame Relay, SONET, ATM, v.11, v.35, v.36, Packet-Over-SONET
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] WIFI Protocols (Detail Only) If one of the following protocols is enabled on the device: 802.11a, 802.11b
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Other Discovery Protocols (Detail Only) If one of the following protocols is enabled on the device: AvayaDP, FDP, CtronDP, EDP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] LAG Protocols (Detail Only) If one of the following link aggregation protocols is enabled on the device: PAGP, LACP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Other STP (Detail Only) If one of the following protocols is enabled on the device: STP, PVST, RPVST+, RSTP, VTP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] MPLS Protocols (Detail Only) If one of the following routing protocols is enabled on the device: LDP, VPLS, RSVP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Other Routing Protocols (Detail Only) If one of the following routing protocols is enabled on the device: EIGRP, RIP, PIM, VPLS, IGMP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] FHRP (Detail Only) If one of the following first hop redundancy protocols is enabled on the device: VRRP, HSRP, ESRP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Tunnel Protocols (Detail Only) If one of the following protocols is enabled on the device: GRE, DMVPN, PPP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Management Protocols (Detail Only) If one of the following protocols is enabled on the device: DHCP, NTP, SNMP, SNMP-TRAPS, Telnet, SFTP, SCP, SSH, HTTP, HTTPS, SOAP, SYSLOG, NETCONF, RESTCONF, RADIUS, TACACS
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Manufacturer Type The type of device (e.g. Firewall, Router, Switch, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor The name of the Vendor who makes this device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model The model of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name The name of the operating system (e.g. IOS, JUNOS, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version The version of the operating system
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] PING Status If the device responds to ping
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] PING Roundtrip (ms) If successful, the roundtrip time in milliseconds for the ping
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] SSH Status If SSH (port 22) is currently enabled and running on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Telnet Status If Telnet (port 23) is currently enabled and running on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] System Up Time How long the device as been running since the last reboot
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen When data for this record was last seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Seen When data for this record was first seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Discovery Source What source this information came from (e.g. Analyzed, CDP, LLDP, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the devices currently being managed and that ITPIE was able to analyze.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Find device *
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the devices that have a management IP of 192.168.1.10
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find device 192.168.1.10
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the devices whose management IP would be contained in the subnet 192.168.1.0/24
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find device 192.168.1.0/24
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the devices whose hostname begins with c4560
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find device c3560*
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] DNS
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns DNS entries for a given ip or fully qualified domain name (FQDN).
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find dns <ip|network|fqdn> history
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP DNS IP An IP Address to match the DNS IP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR DNS IP A CIDR Address to match the DNS IP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <fqdn> Yes Text, MAC, Number FQDN A full or partial query of the fully qualified domain domain name of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] history When used this will display results all the results, not just the most recent one
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] DNS Server IP The management IP of the Active Directory Server
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] DNS IP The management IP of the Active Directory Server
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] FQDN The fully qualified domain name of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Domain Name The domain name of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] DNS Record Type The type of DNS entry (e.g. A, PTR, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Distinguished Name The full location of the device using DN format
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] DNS Changed The date/time this record was changed by DNS
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] DNS Created The date/time this record was created by DNS
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the DNS entries for the IP 172.30.16.9
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find dns 172.30.16.9
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the DNS entries that end with mydomain.net
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find dns *mydomain.net
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the DNS entries that end with mydomain.net
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find dns *mydomain.net history
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Edge
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all MAC records on an edge port for a given network device.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find edge <ip|mac|network>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Remote IP An IP Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR Remote IP A Network Address expressed in CIDR notation (e.g. 192.168.0.0/24 )
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <mac> Yes MAC, Number, Text Remote MAC The MAC Address of the end user device.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] history Displays all results, including records aged out in the system.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote IP The management IP of the remote device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote MAC The MAC address of the remote device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote MAC Registration The OUI registration of the MAC address of the remote device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote MAC Country The Country of Origin from the OUI Registration
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote MAC Type The type of MAC address of the remote device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote Manufacturer Type The type of device (e.g. Firewall, Router, Switch, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote Vendor The name of the Vendor who makes this device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote Platform The name of the platform for the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote Model The model of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote OS Name The name of the operating system (e.g. IOS, JUNOS, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote OS Version The version of the operating system
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote MAC First Seen When data for this record was first seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote MAC Last Seen When data for this record was first seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor The name of the Vendor who makes this device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Platform The name of the platform for the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model The model of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name The name of the operating system (e.g. IOS, JUNOS, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version The version of the operating system
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] System Up Time How long the device as been running since the last reboot
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Name The interface the host is attached to
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Description The description of the interface on the local device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Status The status of the interface on the local device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Speed The speed of the interface on the local device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Last Change Seconds The time of the last change of the interface statistics
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface VLAN Count The number of tagged VLANs on the interface connected to the local device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface MAC Count The number of MAC addresses on the interface connected to the local device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VRF Name The VRF configured on the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Network Prefix The containing subnet for the remote IP (e.g. 1.1.1.0/24 )
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN ID The VLAN ID configured on the interface this host was attached to
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN Name The VLAN name configured on the interface this host was attached to
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Manufacturer Type The type of device (e.g. Firewall, Router, Switch, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the edge ports for devices whose management IP matches 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find edge 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the edge ports for devices whose MAC matches 00:00:5E:00:53:FF
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find edge 00:00:5E:00:53:FF
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the edge ports for devices contained in network 192.168.0.0/24
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find edge 192.168.0.0/24
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Host
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all host records matching given terms.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find host <hostname|ip|network|mac>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Remote IP An IP Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR Remote IP A Network Address expressed in CIDR notation (e.g. 192.168.0.0/24 )
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <mac> Yes MAC MAC The MAC Address of the device.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <hostname> Yes Text, Number Hostname, MAC The Hostname or partial MAC of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor The name of the Vendor who makes this device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Platform The name of the platform for the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model The model of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name The name of the operating system (e.g. IOS, JUNOS, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version The version of the operating system
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Manufacturer Type The type of device (e.g. Firewall, Router, Switch, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Serial Number The serial number for the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Discovery Source How the device was discovered (ARP, SSH analysis, etc.)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Mac Mac address of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen Last time the device was found by a collection
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the hosts for devices whose management IP matches 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find host 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the devices whose hostname matches c3560*
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find host c3560*
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the devices contained in network 192.168.0.0/24
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find host 192.168.0.0/24
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns the device with the mac address 00:00:5E:00:53:FF
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find host 00:00:5E:00:53:FF
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find int[erface]|port|ifc <ip|network|desc> find int[erface]|port|ifc <ip|network|desc> det[ail] find int[erface]|port|ifc <ip|network|desc> ip
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields Default and Detail
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields ID
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Device IP Returns all the records associated with the Device IP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR Device IP Returns all the records whose Device IP is contained in the provided CIDR
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <desc> Yes Text, Number, MAC Description All or part of the description of an interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] detail Adds addtional columns to the result set
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] ip Also shows the list of IP Addresses, if any, assigned to the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Logical System Name The name of the logic system if applicable
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface The name of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Description The description of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VRF Name The VRF configured on the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Admin Status The configured status of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Oper Status The operational status of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Admin Speed The configured speed of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Oper Speed The operational speed of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Admin Duplex The configured duplex of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Oper Duplex The operational duplex of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] POE Power Consumption (mw) The operational duplex of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Tranceiver Type The type of tranceiver if applicable (e.g. Fixed, SFP, QSFP)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Cable Type The type of cable (e.g. Copper, Single-Mode Fiber, Multi-Mmode Fiber, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Medium The medium of the cable(e.g. Copper, Fiber)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Medium Type The type of cable medium (e.g. Single-Mode, Multi-Mmode, Twinaxial, Twisted Pair, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface IPs The IPs assigned to the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] MAC (Detail Only) The MAC address of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Admin VLAN Port Mode (Detail Only) The VLAN Port mode of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Type (Detail Only) The type of interface (e.g. Ethernet, EtherSVI, Tunnel, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Change (Detail Only) The last time a change was detected of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Logical System Name The name of the logic system if applicable
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface The name of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VRF Name The VRF configured on the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface IPs The IPs assigned to the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Oper Status The operational status of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Oper Speed The operational speed of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Oper Duplex The operational duplex of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Description The description of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the interfaces whose description contains the value loopback
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find interface *loopback*
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Inventory
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find inv[entory]|hard[ware] <ip|network|serial|productid|name|desc>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR Device IP A network expressed in CIDR notation (e.g. 192.168.0.0/24 )
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <serial> Yes Text, Mac, Number Product Serial Number All or part of a serial number found on a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <product_id> Yes Text, Mac, Number Product ID All or part of a product ID found on a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <name> Yes Text, Mac, Number Product Name All or part of a name of a piece of hardware found on a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <desc> Yes Text, Mac, Number Product Description All or part of a description of a piece of hardware found on a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor The name of the Vendor who makes this device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model The model of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name The name of the operating system (e.g. IOS, JUNOS, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version The version of the operating system
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Discovery Source The source of the information. (e.g. Analysis or User Provided)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Product Name The name of the product
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Product Description The description of the product
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Product Serial Number The serial number of the product
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Product ID The product id or product number
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Product Part Number (Detail Only) The product number
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Longitude The logitude
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Latitude The latitude
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] FRU Is this a Field Replacable Unit
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Virtual Is this a virtual item
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen When data for this record was last seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Seen When data for this record was first seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Position Index (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the inventory records whose device has a management IP of 192.168.1.10
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find inventory 192.168.1.10
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the inventory records whose device has management IP would be contained in the subnet 192.168.1.0/24
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find inventory 192.168.1.0/24
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the inventory records whose serial number begins with sn1234
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find inventory sn1234*
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the inventory records whose product ID is 1234
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find inventory 1234
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the inventory records whose name contains cisco
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find inventory *cisco*
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the inventory records whose description contains 24
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find inventory *24*
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Link Aggregation Group (LAG)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns information about the virtual interface bundles, and associated physical interfaces, configured on a device.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find lag <ip|hostname>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Device IP IP Address of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <hostname> Yes Text, Number Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Logical System The logical system name of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor The name of the Vendor who makes this device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS The name of the operating system (e.g. IOS, JUNOS, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model The model of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] LAG Protocol The type of LAG protocol used on the link (e.g. LACP, VPC, PAGP, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] LAG Mode The operational mode of the LAG interface (e.g. L2, L3, , etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] LAG Interface The name of the LAG interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] LAG Status The operational status of the LAG interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] LAG Speed The operational speed of the LAG interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] LAG Duplex The operational duplex of the LAG interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Member Interface The name of the member interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Member Status The operational status of the member interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Member Speed The operational speed of the member interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Member Duplex The operational duplex of the member interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all virtual LAG interface bundless on device 10.110.20.190 , the associated member ports, and the status of the virtual and physical interfaces.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find lag 10.110.20.190
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Note: This report does not currently distinguish between a normal LAG versus a Multi-Chassis LAG (MC-LAG).
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] License
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns information about device licenses. Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find license <ip|vendor>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Device IP IP Address of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <vendor> Yes Text Vendor The vendor of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor The name of the Vendor who makes this device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model The model of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS The name of the operating system (e.g. IOS, JUNOS, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version The version of the operating system
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device Manufacturer The type of device (e.g. Firewall, Router, Switch, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Description The description of the license
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Part Number The part number of the license
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] License Type The type of the license
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] License Name The name of the license
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Days Until Expiration The number of days until the license expires
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Percentage Used The percentage of the license that has been used
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Quantity Available The quantity of licenses available
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Quantity in Use The quantity of licenses used
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Start Date The start date of the license
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] End Date The expiration/end date of the license
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples Returns all license information for device with IP 10.110.20.190 .
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find license 10.110.20.190
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all license information for device with vendor VMware .
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find license VMware
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Log (Cisco ISE log)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns information about Cisco ISE TACACS live logs. For more details about these fields, see the Cisco documentation .
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find log <ip|hostname>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Device IP IP Address of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <hostname> Yes Text, Number Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device requesting TACACS authentication
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] ISE Node The name of the ISE node that is processing the request
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote Address The IP of the device trying to log in
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Shell Profile The privileges granted to the user for executing commands on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Status The success or failure of the authorization/authentication
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Failure Reason If the login failed, then why it failed
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Type Either all, authentication, or authorization
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Username The username of the login
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Authentication Policy The name of the authentication policy being applied
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Authorization POlicy The name of the authorization policy being applied
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device Port The port that the remote device is accessing on the network device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device Type The device type policy that is used to process access requests
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Location The location-based policy that is used to process the request
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Matched Command Set The command set that the logged in user is allowed
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Logged Time The time the event was registered
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns Cisco TACACS live log information for access to device 10.110.20.190 .
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find log 10.110.20.190
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] MAC
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns information about MAC Addresses.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] The default command returns a single record for an IP or MAC if that IP or MAC exists as an end user device in ITPIE.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] The all option will return all of the MAC entries from each network device that match the provided criteria.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] The edge option will return all edge records that match the provided search criteria.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find mac|host|ip <ip|mac> all|edge|history
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find mac
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find mac|host|ip <ip|mac>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Default Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP ARP IP The IP address of the end user device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <mac> No MAC, Text, Number MAC The MAC address of the end user device.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] MAC Wildcard Support
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Wildcard suport for the <mac> predicates is supported for the all , edge and history options, but not for the main find mac 00:00:5E:00:53:FF syntax. This is temporary. We are looking to add wildcard support in the near future.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface The interface the host is attached to
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Bridge Detected If a bridge was detected between the host and the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] MAC The MAC address of the host
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Registration The OUI registration of the MAC address of the host
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] ARP IP The IP address of the host as seen by ARP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VRF Name The VRF the host is currently on
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Description The description of the interface the host is attached to
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN Name The name of the VLAN configured on the interface this host was attached to
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN ID The VLAN ID configured on the interface this host was attached to
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] MAC48 Type The type of MAC address of the host
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen When data for this record was last seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns information about the device that has the IP 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find mac 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns information about the device that has the MAC 00:00:5E:00:53:FF
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find mac 00:00:5E:00:53:FF
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find mac * all
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find mac|host|ip <ip|mac|hostname> all
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] All Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Device IP The Management IP address of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <mac> Yes MAC MAC The MAC address of the end user device.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <hostname> Yes Text, Number Hostname, MAC The hostname or partial MAC of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] all Returns all the MAC addresses in the MAC address table for the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Logical System Name The name of logical system
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface The interface the host is attached to
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Description The interface description the host is attached to
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN ID The VLAN ID configured on the interface this host was attached to
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN Name The VLAN Name configured on the interface this host was attached to
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Registration The OUI registration of the MAC address of the host
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OUI Country The Country associated with the OUI Registration
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] MAC The MAC address of the host
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Is Unique
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Unique MAC Count The number of macs that are considered unique (i.e. Not from a pool of known, duplicated MACs)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Seen From The Date/Time this record was first seen in this form
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Seen To The Date/Time this record was last seen in this form
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Tip
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] "Pro Tips!"
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] You can search for partial MACs using wildcards ( * )
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Partial MAC searches must meet the following criteria
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Currently only supported with find mac * all
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] May use Trailing OR Leading & Trailing wildcards
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Only supports the MAC format xx:xx:xx:xx:xx:xx , x may be replaced by any valid entry [0-9|a-f|A-F]
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Requires at least two full octects plus a trailing :
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find mac *5f:bf:* all
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the MAC Address table entries for the network device that has the IP 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find mac 1.2.3.4 all
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find mac * history
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find mac|host|ip <ip|mac|hostname> history
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] All Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Device IP The Management IP address of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <mac> Yes MAC MAC The MAC address of the end user device using : delimited format 00:00:5E:00:53:FF
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <hostname> Yes Text, Number Hostname, MAC The hostname or partial MAC of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] history Returns all the MAC addresses in the MAC address table for the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Please refer to the mac all report fields.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns historic records for the MAC Address table entries for the network device that has the IP 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find mac 1.2.3.4 history
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find mac * edge
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find mac|host|ip <ip|mac> edge
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] See the find edge command for supported predicates and report fields.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Media
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns information about the physical port media on interfaces.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find me[dia] <ip|network|mediatype>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Device IP IP Address of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR Device IP CIDR based network filter for a set of IP Addresses of devices
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <mediatype> Yes Text, MAC, Number Tranceiver Type, Physical Media Spec, Connector Type, Cable Type A full or partial value from one of the matched fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor The name of the Vendor who makes this device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS The name of the operating system (e.g. IOS, JUNOS, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model The model of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Name The name of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Tranceiver Type The type of tranceiver, if applicable (e.g. Fixed, SFP, QSFP, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Cable Type The type of cable (e.g. Copper, Singlemode Fiber, Multimode Fiber, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Cable Medium The medium of the cable(e.g. Copper, Fiber)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Cable Medium Type The type of cable medium (e.g. Single-Mode, Multi-Mmode, Twinaxial, Twisted Pair, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Physical Media Spec The physical media specification (e.g. 10/100/1000BASE-TX, 10GBASE-LR, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Cable Medium Description Additional information about the cable medium
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Modulation What modulation is being used: Baseband, Broadband, Bandpass
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Speed What speed is the cable rated for
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] PCS Physical coding layer
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] PCS Description Description of the physical coding layer
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Reach How far the cable is rated
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Type The type of interface (e.g. Ethernet, EtherSVI, Tunnel, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Description The configured description of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VRF Name The VRF configured on the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Oper Status The operational status of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Admin Status The configured status of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Oper Speed The operational speed of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Admin Speed The configured speed of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Oper Duplex The operational duplex of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Admin Duplex The configured duplex of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Seen When data for this record was first seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen When data for this record was last seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the interfaces with a transciever type of sfp
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find media sfp
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Neighbors
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the logical Layer 1 adjacencies for a given network device.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find nei[ghbor] <ip|network|hostname> find nei[ghbor] <ip|network|hostname> det[ail]|tag[ged]
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR Device IP A network in CIDR notation
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <hostname> Yes Text, MAC, Number Hostname All or part of the hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] detail Adds additional fields to the returned data of the query
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] tagged Adds additional fields related to the number of tagged VLANs on the interface connected to the remote device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Discovery Type The kind of discovery protocol used to find this neighbor (e.g. LLDP, CDP, FDP, EDP, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface The name of the interface on this device that is connected to the remote device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Desc The configured descriptoin of the interface connected to the remote device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface VLAN Count (Tagged/Detail Only) The number of tagged VLANs on the interface connected to the remote device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote Device IP The IP of the remote device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote Hostname The hostname of the remtoe device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote Interface The name of the interface on the remote device that is connected to the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote Interface Desc The description of the interface on the remote device that is connected to the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote Manufacturer Type The type of remote device (e.g. Firewall, Router, Switch, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote Serial Number The serial number for the remote device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote Vendor The name of the Vendor who makes the remote device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote Model The model of the remote device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote OS Name The name of the operating system on the remote device (e.g. IOS, JUNOS, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote OS Version The version of the operating system on the remote device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote Is Unmanaged Indicates if the remote device is currently being managed by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote Last Seen When data for this remote device was last seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Remote First Seen (Detail Only) When data for this remote device first seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the neighbors for devices whose management IP matches 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find neighbor 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the neighbors for devices whose hostname matches c3560-corp-1
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find neighbor c3560-corp-1
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] NetBIOS
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns NetBIOS Name information
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find netb[ios]|nb <ip|network|name>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Network Smallest Network Prefix containing the provided IP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR Network List of all Network Prefixes contained in the provided subnet
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <name> Yes Number, Text, MAC VRF A full or partial value from one of the matched fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Collected IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Net BIOS Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Source Net BIOS Source
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Is Truncated Indicates if the name was truncated (because it was too long to fit in 32 characters)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Is Group Indicates if the Name record is a group (i.e. a domain name)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Is Active Indicates if the name is currently active.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Is Permanent Indicates if the name is permanent
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Is In Conflict Indicates if the name is in conflict.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Is Being Deregistered Indicates if the name is being deregistered.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Owner Node Type The type of node that owns the name: Broadcast, Point2Point, Mixed, Reserved
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Seen When the name was first seen.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen When the name was last seen.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns NetBIOS names for the provided ip
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find netbios 1.1.1.1
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns NetBIOS names that start with corp .
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find netbios corp*
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Network
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns a list of unique Network Prefixes by VRF with some statistics.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find net[work] <ip|cidr|vrfname>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Network Smallest Network Prefix containing the provided IP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <cidr> No CIDR Network List of all Network Prefixes contained in the provided subnet
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <vrfname> Yes Text, MAC VRF A full or partial value from one of the matched fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Network The CIDR notation of the Network Prefix
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VRF The name of the VRF the Network Prefix is assigned to
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Utilization The percentage of the network in use
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hosts in Use The name of IPs in use contained in the Network Prefix
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Network Devices Configured with Network The number of network devices with the Network Prefix / VRF pair configured
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns the network 10.110.10.0/23 which contains the IP 10.110.10.67
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find network 10.110.10.67
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns the list of network prefixes by VRF contained the subnet 10.110.0.0/16
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Network Prefix VRF Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] 10.110.10.0/23 Mgmt-intf
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] 10.110.20.0/23 org-mgmt-dmz
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] 10.110.20.0/24 trust-vr
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] 10.110.101.0/24 management
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] 10.110.101.0/24 Mgmt-intf
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find network 10.110.0.0/16
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns the list of networks assigned to the VRF sdev-test-tr
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find network 10.110.10.67
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns information about phones seen on the network.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find ph[one] <phone_ip|phone_number|phone_mac> detail|tdm|location|all
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields Default
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields TDM
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields Location
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields All
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <phone_ip> No IP Phone IP The IP of the VOIP phone trying to be located
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <phone_network> No CIDR Phone IP The Network address in CIDR notation for the IP of the VOIP phone trying to be located
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <phone_number> Yes Number Phone Number The number of the phone trying to be located
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <phone_mac> Yes MAC, Text The MAC of the VOIP phone trying to be located The MAC Address of the phone tying to be located.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface The Interface of the network device to which the VOIP phone is attached
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Desc (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] POE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN The VLAN ID configured on the Interface of the network device to which the VOIP phone is attached
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VRF Name (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone Number The Number of the Phone
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone IP The IP of the VOIP Phone
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone MAC The MAC of the VOIP Phone
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone Location The physical location of the Phone
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone Vendor (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone Model (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Discovery (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone Protocol The protocol used to discover the Phone
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen (Detail Only) The date/time the phone was last seen
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Seen (Detail Only) The date/time the phone was first seen
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone Number The Number of the Phone
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] TDM Port
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone Key #
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] TDM Phone Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone Number The Number of the Phone
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone Location The physical location of the Phone
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] House #
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Street
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] State
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Bldg
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Room
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Desc
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface The Interface of the network device to which the VOIP phone is attached
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Desc
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] POE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN The VLAN ID configured on the Interface of the network device to which the VOIP phone is attached
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VRF Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone Number The Number of the Phone
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone IP The IP of the VOIP Phone
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone MAC The MAC of the VOIP Phone
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone Location The physical location of the Phone
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone Vendor
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone Model
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Discovery
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone Protocol The protocol used to discover the Phone
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] TDM Port
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone Key #
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] TDM Phone Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] House #
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Street
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] State
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Bldg
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Room
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen The date/time the phone was last seen
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Seen The date/time the phone was first seen
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the phones that match the IP 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find phone 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the phones that match the phone number (123) 456-7890
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find phone 1234567890
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the phones that match the MAC 00:00:5E:00:53:FF
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find phone 00:00:5E:00:53:FF
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Port Status
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns a list of ip addresses and status on specific open ports (22, 80, 443, Ping, and NetBios).
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find ports[tatus]|dps <ip|network|status>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Collected IP Smallest Network Prefix containing the provided IP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <cidr> No CIDR Collected IP List of all Network Prefixes contained in the provided subnet
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <status> Yes Text Status (HTTP, HTTPS, SSH, NETBIOS, PING) A full or partial value from one of the matched fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Collected IP IP address that was tested.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Protocol Name The name of the protocol
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Port Number The TCP port number tested (empty for ICMP)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Status The IPStatus or Socket Error of an attempt to connect to the TCP port or to send an Internet Control Message Protocol (ICMP) echo request and receive the corresponding ICMP echo reply message.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Value Type A description of what the Value column indicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Value The value described by the Value Type column
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Seen The first time the protocol was tested for this IP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen The last time the protocol was tested for this IP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns the port status record for that ip.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find portstatus 10.110.10.67
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the port status records for ips that are in the subnet 10.110.0.0/16
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find dps 10.110.0.0/16
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Power
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns information for PDU and UPS devices
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find pow[er]|pwr <ip|hostname> input|outlet
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields Outlet
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields Input
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP, CIDR Device IP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <hostname> Yes Number, MAC, Text Hostname
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Manufacturer Type The type of device (e.g. Firewall, Router, Switch, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor (Detail Only) The name of the Vendor who makes this device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model (Detail Only) The model of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name The name of the operating system (e.g. IOS, JUNOS, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version (Detail Only) The version of the operating system
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Input Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Feed Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Plug Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Frequency Within Tolerance
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Feed Color
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phase Count
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phase Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Max Current Rating (amps)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Max Phase Current Rating (amps)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Max Power Rating (watts)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Load Status
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Snapshot Power Consumption (watts)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Snapshot Apparent Power Consumption (volt-amps)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Snapshot Power Factor
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Peak Power Consumption (watt hours)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Peak Power Consumption Timestamp
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Peak Power Consumption Reset
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Running Energy Total (watt hours)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Running Energy Total Reset
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Unit Position Index
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Unit User Index
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Input Index
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Seen
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Manufacturer Type The type of device (e.g. Firewall, Router, Switch, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor (Detail Only) The name of the Vendor who makes this device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model (Detail Only) The model of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name The name of the operating system (e.g. IOS, JUNOS, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version (Detail Only) The version of the operating system
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Outlet Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Receptacle Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Max Power Rating (watts)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Switch Status
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phase Layout
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Load Status
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Snapshot Current
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Snapshot Power Consumption (watts)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Snapshot Apparent Power Consumption (volt-amps)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Snapshot Power Factor
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Peak Power Consumption (watt hours)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Peak Power Consumption Timestamp
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Peak Power Consumption Reset
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Running Energy Total (watt hours)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Running Energy Total Reset
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Unit Position Index
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Unit User Index
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Outlet Index
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Seen
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns power outlet information for devices matching the ip address.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find power 1.1.1.1 outlet
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns power input information for devices matching the ip address.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find power 1.1.1.1 input
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Protocol
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns information about what protocols devices are running (as either a client or a server)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns which protocols are running on a device.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find prot[ocol] <protocol_category> Mgmt|L1+Link|L2|Routing
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns information about which network services a device is configured to use.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find prot[ocol] <protocol> Associations
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Association Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <protocol_category> Yes MGMT, L1+link, L2, or routing (these are case insensitive)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <protocol> Yes NTP, DNS, TACACS, etc...
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS The name of the operating system
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Logical System The system's uniquely identifiable name within the network
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Protocol The protocol used to discover the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Operating Status Last known running status
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Admin Status The configurted status
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Protocol Role Protocol role (e.g. Client, Server)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Protocol Category Protocol category (e.g. MGMT, L1+link, L2, or routing)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] L4 Protocol The OSI Layer 4 Protocol (e.g. TCP, UDP, ICMP, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Port The active port of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen When data for this record was last seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Logical System The system's uniquely identifiable name within the network
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Protocol The protocol used to discover the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Protocol Category Protocol category (e.g. DNS, SNMP, Time, Name, Authentication, DHCP, File)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Service IP The IP Address of the service the device is configured to use.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Port The active port of the service
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen When data for this record was last seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns device information for devices matching the SSH protocol.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find protocol ssh
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns device associations for protocols.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find protocol * associations
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Route
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find rou[te] <ip|prefix> find rou[te] <ip|prefix> all find rou[te] <ip|prefix> ex[act] find rou[te] <ip|prefix> vrf <routing-instance|vrf>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Route Prefix The IP you wish to find matching routes for
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <prefix> No CIDR Route Prefix (Exact match, not results found within CIDR) A network address expressed in CIDR notation (e.g. 10.100.0.0/24 )
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <routing-instance> Yes Text, MAC, Number Routing Instance ( vrf option only) The name of a routing instance
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <vrf> Yes Text, MAC, Number Routing Instance ( vrf option only) The name of a VRF
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] all Returns all matching routes for the provided IP or Prefix
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] exact Returns routes that match the exact IP or Prefix provided
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] vrf Return routes that match the provided IP or Prefix from VRFs that match the Routing-Instance or VRF
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Logical System Name The name of the logical system
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Routing Instance The name of the routing instance
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Route Prefix
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Route Source
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Pref/Metric
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Next Hop IP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Next Hop Interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] BGP AS Path
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] BGP Local Pref
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Seen From The Date/Time this record was first seen in this form
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Seen To The Date/Time this record was last seen in this form
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the route entries that match the IP 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find route 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the route entries that match the network address 1.2.3.0/24
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find route 1.2.3.0/24
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Software Packages
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns software package data collected via the WMI/SSH collection types using the ITPIE Collection Engine (GUI or CLI).
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find soft[ware] <ip|network|packagename>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP IP Address The IP Address of a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR IP Address A network address in CIDR notation that includes the IP Address of a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <packagename> Yes Text, MAC, Number Package Name A full or partial package name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The IP Address used to collect on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The reported Hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Platform
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Manufacturer Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Package Name The name of the package.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Package Version The version of the package
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Package Vendor THe package vendor
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Package Summary A longer description of the package.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Package Install Date When the package was installed.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Package Install Source File The location of the source file for the installer.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Package Code
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Package URL
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Package Maintainer
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Package Architecture
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Package Size
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Package Signature
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Package Version Long
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Package License
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Package Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Package Long Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Package First Seen
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Package Last Seen
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all software packages whose Package Name matches perl exactly
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find software perl
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all software packages whose Package Name contains perl
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find software *perl*
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Spanning Tree
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find stp|span[ning-tree] <vlan_id|mst_id|bridge_address|ip|network|hostname> find stp|span[ning-tree] <vlan_id|mst_id|bridge_address|ip|network|hostname> det[ail] find stp|span[ning-tree] <vlan_id|mst_id|bridge_address|ip|network|hostname> int[erface]|port|ifc
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields Default and Detail
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <hostname> Yes Text Hostname All or part of the Hostname or Bridge Address of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <vlan_id> No Number VLAN Range A VLAN ID (a number between -1 and 4095) used by Spanning Tree
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <mst_id> No Number MST Instance ID An MST Region ID
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <bridge_address> Yes MAC Bridge Address A Spanning Tree node's Bridge Identifier, usually in the form of a MAC address (e.g. 00:00:5E:00:53:FF )
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] detail Adds additional fields to the returned data of the query
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] interface Returns the data at the interface level instead of just listing the nodes on a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Manufacturer Type The type of device (e.g. Firewall, Router, Switch, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor (Detail Only) The name of the Vendor who makes this device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model (Detail Only) The model of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name The name of the operating system (e.g. IOS, JUNOS, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version (Detail Only) The version of the operating system
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] STP Type (Detail Only) The type of protocol the Spanning Tree instance is using
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] STP Name The name of the Spanning Tree instance
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] STP Instance ID
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] STP Revision (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Admin Status (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN Range
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Bridge Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Bridge Priority
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Root Bridge (RB)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] RB IP The IP of the Root Bridge
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] RB Hostname The hostname of the Root Bridge
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] RB Priority
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] RB Path Cost
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] RB Port
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Regional RB (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Regional RB Priority (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Is Root (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] TCN Flag Set (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] TCN Flag Detected (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Forward Delay (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hello Time (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Max Age (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Topology Change
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen (Detail Only) When data for this record was last seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Seen (Detail Only) When data for this record was first seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Manufacturer Type The type of device (e.g. Firewall, Router, Switch, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name The name of the operating system (e.g. IOS, JUNOS, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface The name of the interface Spanning Tree is configured on
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] STP Protocol
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] STP Instance ID
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN Range
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Bridge Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Bridge Priority
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Is Root
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Role
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Status
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Oper Port Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Designated Bridge (DB)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] DB Path Cost
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] DB Port Number
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] DB Priority
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Is Designated Remote
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen When data for this record was last seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Seen When data for this record was first seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the Spanning Tree nodes for devices whose management IP matches 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find stp 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the Spanning Tree nodes for devices whose hostname matches c2911-corp-1
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find stp c2911-corp-1
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the Spanning Tree nodes that are running on the VLAN or MST ID that matches 3
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find stp 3
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the Spanning Tree nodes whose bridge addresss matches 00:00:5E:00:53:FF
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find stp 00:00:5E:00:53:FF
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] SSH Negotiation Info
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find ssh <ip|network|hostname|server_id|key_exchange_algorithm|host_key_algorithm|signature_algorithm> find ssh <ip|network|hostname|server_id|key_exchange_algorithm|host_key_algorithm|signature_algorithm> det[ail]
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields Default and Detail
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Host The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR Host The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <server_id> Yes Text, MAC, Number Server Identification
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <key_exchange_algorithm> Yes Text, MAC, Number Key Exchange Algorithm/Cipher ID
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <host_key_algorithm> Yes Text, MAC, Number Host key Algorithm/Cipher ID
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <signature_algorithm> Yes Text, MAC, Number Signature Hash Algorithm
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] detail Adds additional fields to the returned data of the query
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Host The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Port The port ssh connected on
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Server Fingerprint The SSH Server's fingerprint
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Server Identification The SSH Server's identification banner
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Signature Hash Algorithm The algorithm used to produce the hash used to verify the signature of the SSH Server
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Host Key Cipher ID The Cipher ID used to produce the Host Key
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Host Key Algorithm The Algorithm used to produce the Host Key
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Key Exchange Cipher ID The Cipher ID used to produce the Key Exchange
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Key Exchange Algorithm The Algorithm used to produce the Key Exchange
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Incoming Encryption Cipher ID (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Incoming Encryption Mode (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Incoming Encryption Algorithm (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Incoming Compression Enabled (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Incoming Mac Cipher ID (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Incoming Mac Algorithm (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Outgoing Encryption Cipher ID (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Outgoing Encryption Mode (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Outgoing Encryption Algorithm (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Outgoing Mac Cipher ID (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Outgoing Mac Algorithm (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Outgoing Compression Enabled (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Compression Algorithms Client to Server (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Compression Algorithms Server to Client (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Encryption Algorithms Client to Server (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Encryption Algorithms Server to Client (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Key Exchange Algorithms (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Mac Algorithms Client to Server (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Mac Algorithms Server to Client (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Server Host Key Algorithms (Detail Only)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen When data for this record was last seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Seen When data for this record was first seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the ssh negotiation info for devices whose management IP matches 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find ssh 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the ssh negotiation info for server ids that contain ssh 2
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find ssh *ssh 2*
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Tunnel
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] A list of tunnel interfaces that match the user provided query.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find tunnel <ip|network|interfacename>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP IP Address The IP Address of a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR IP Address A network address in CIDR notation that includes the IP Address of a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <interfacename> Yes Text Interface Name A full or partial interface name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The IP Address used to collect on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The reported Hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Logical System Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface VRF
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface IP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Tunnel Interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Tunnel VRF
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Tunnel IP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Tunnel Port
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Dest. IP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Dest. Port
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Tunnel Key
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Encapsulation
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Security
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] MTU
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find tunnel 192.0.2.0/24 find tunnel 192.0.2.5 find tunnel Cisco\*
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find vl[an] <vlan_id|hostname|ip|network> find vl[an] <vlan_id|hostname|ip|network|vlan_name> de[vice] find vl[an] <vlan_id|hostname|ip|network> int[erface]|port|ifc
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR Device IP A network address in CIDR notation that matches the management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <vlan_id> No Number VLAN IDs A VLAN ID (a number between -1 and 4095)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <hostname> Yes Text Hostname All or part of a Hostname
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <vlan_name> Yes Text Vlan name All or part of a Vlan name (only works for device searches)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] device Adds additional fields to the returned data of the query
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] interface Returns the data collated at the interface level instead of listing the VLANs individually for the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface The name of the Interface the VLAN is configured on
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VRF Name The configured VRF for the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Admin Port Mode
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN IDs The VLAN IDs configured and allowed on the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN Attribute
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN Filter The VLANs allowed on the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN Filter Action
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN Filter Direction
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Oper Status Operational status of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Status Time
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen When data for this record was last seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Logical System Name The name of the Logical System, if applicable
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor The Vendor of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name The name of the operating system running on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN ID
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN Attribute
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Admin Status
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model The model of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Platform The platform of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version The version of the operating system running on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Manufacturer Type The type of device (e.g. router, switch, firewall, etc...)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen (Detail Only) When data for this record was last seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Seen (Detail Only) When data for this record was first seen by ITPIE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the VLANs configured on devices whose management IP matches 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find vlan 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the VLANs whose device hostname matches corp-1
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find vlan corp-1
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the VLANs from devices whose VLAN ID match 200
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find vlan 200
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VRF
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find vrf <name|ip|network> find vrf <name|ip|network> lo[opback]
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Interface IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR Interface IP A network address expressed in CIDR notation (e.g. 192.168.32.0/24 )
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <name> Yes Text, MAC, Number VRF Name All or part of a VRF name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] loopback Returns only the loopback interfaces
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Logical System name The name of the logical system
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VRF Name The name of the VRF configured for this interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Route-Distinguisher (RD)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Network Prefix
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface The name of the Interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface IP The IP address configured on the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Network Mask The Mask of the IP address configured on the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Type The type of interface (e.g. Ethernet, EtherSVI)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface VLAN The VLAN configured on the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface VLAN Name The VLAN Name configured on the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] FHRP Status
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Route-Target(s) (RT)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Node Forwarding Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Description The description of the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the interfaces that have an IP that matches 1.2.3.4 configured on the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find vrf 1.2.3.4
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the interfaces that have an IP that matches the nework 1.2.3.0/24 configured on the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find vrf 1.2.3.0/24
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the interfaces that a VRF that matches corp-vpn configured on the interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find vrf corp-vpn
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Third Party Integration Commands
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Aruba ClearPass
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns host information known from integration with Aruba ClearPass
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find arubaclearpass|acp <hostip|cidr|hostname|fingerprintname>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <host_ip> No IP Device IP IP Address of a host known to Aruba ClearPass
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <cidr> No CIDR Device IP CIDR for a group of a hosts known to Aruba ClearPass
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <hostname> Yes Text, MAC, Number Device Hostname Hostname of a host known to Aruba ClearPass
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <fingerprintname> Yes Text, MAC, Number Fingerprint Name Name of the fingerprint
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device MAC
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device Hostname
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Fingerprint Category
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Fingerprint Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Fingerprint Updated At
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Fingerprint Added At
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Source ClearPass Server
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Record Created On
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Record Updated On
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns record whose Device IP matches 1.1.1.1
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find arubaclearpass 1.1.1.1
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Cisco DNAC Devices
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns host information known from integration with Cisco DNAC Devices
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find cisc[odnacdevice]|dnac <ip>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP Ip The ip address of a device known to Cisco DNAC
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <cidr> No CIDR Ip CIDR of a group of devices known to Cisco DNAC
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Management IP Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] AP Manager Interface IP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Associated WIC IP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] AP Ethernet MAC Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] MAC Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Family
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Memory Size
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device Support Level
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Software Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Software Version
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Serial Number
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Collection Interval
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Management State
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Inventory Status Detail
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Role Source
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Collection Status
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Location Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Platform ID
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Reachability Failure Reason
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Reachability Status
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Series
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] SNMP Contact
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] SNPM location
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Error Code
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Error Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Interface Count
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Line Card Count
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Line Card ID
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Tag Count
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Tunnel UDP Port
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] WAAS Device Mode
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Location
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Role
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Instance Tenant ID
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Instance UUID
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device ID
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Managed At Least Once
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Uptime Seconds
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Update Time
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Updated
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Boot Date Time
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Created On
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the Cisco DNAC devices whose address is in the 1.1.1.0/24 subnet.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find ciscodnacdevice 1.1.1.0/24
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Cisco ISE Devices
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns host information known from integration with Cisco ISE Devices
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find ised[evices] <name>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <name> Yes Text, MAC, Number, IP, CIDR Name The name of a device known to Cisco ISE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Version
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Subnets
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the cisco ise devices whose Name matches foo .
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find isedevices foo
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Cisco ISE Sessions
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns a list of known Cisco ISE sessions
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find ises[essions] <host_mac|host_ip|username>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <host_ip> No IP Host IP Address The IP of a device known to Cisco ISE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <host_network> No CIDR Host IP Address A network addresss in CIDR notation that includes the IP of a device known to Cisco ISE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <host_mac> Yes Text, MAC, Number Host MAC Address The MAC of a device known to Cisco ISE
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <username> Yes Text, MAC, Number Username, Host MAC Address The username of a user known to Cisco ISE , or parital MAC od a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Host MAC Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Host IP Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Username
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device Hostname
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Authentication Method
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Authentication Protocol
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the Cisco ISE sessions whose Username matches first.last .
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find isesessions first.last
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] iBoss Host
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns Host records known to iBoss.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find iboss <host_ip> cloud find iboss <host_ip> static find iboss <host_ip> anonymous find iboss <host_ip> all
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <host_ip> No IP IP Address IP Address of the host device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] cloud Finds iBoss cloud hosts
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] static Finds iBoss statically-defined hosts
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] anonymous Finds iBoss anonymous hosts
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] all Finds iBoss hosts of any type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device Location
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Asset Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] User Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Seen
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Score
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Expired Time
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen IP
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen Location
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Is Missing
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Is Active
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Agent Version
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Registration Info
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Critical OS Patches
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Firewall Enabled
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Disk Encrypted
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Anti-malware
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns iBoss static records whose IP Address matches 1.1.1.1 .
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find iboss 1.1.1.1 static
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Infoblox Host
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns Host records known to Infoblox.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find infoblox <host_ip|host_network|host_mac> host
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <host_ip> No IP IP Address IP Address of the host device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <host_network> No CIDR IP Address A network address in CIDR notation that matches the IP Address of a host device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <host_mac> Yes Text, MAC, Number MAC Address A full or partial mac address for the host device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] host
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Infoblox Server IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Status
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] IP Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Network
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] MAC Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] MGMT IP Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] NetBIOS Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Contact
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Location
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Discovered Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Discoverer
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Discovered
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Discovered
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Created On
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Updated On
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns Infoblox Host records whose IP Address matches 1.1.1.1 .
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find infoblox 1.1.1.1 host
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Infoblox Network
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns IPAM Network records known to Infoblox.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find infoblox <network> network
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR IP Address A network in CIDR notation that includes the IP Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] network
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Infoblox Server IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Status
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] IP Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Created On
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Updated On
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns Infoblox Network records whose IP Address matches or is a subset of 1.1.1.0/24 .
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find infoblox 1.1.1.0/24 network
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Infoblox VLAN
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns IPAM VLAN records known to Infoblox.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find infoblox <vlan_id|vlan_name> vlan
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Options
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <vlan_id> No Number VLAN ID A VLAN ID (a number between -1 and 4096)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <vlan_name> Yes Text, MAC, IP, CIDR Name A full or partial VLAN Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] vlan
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Infoblox Server IP The management IP of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] VLAN ID
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Reserved
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Status
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Comment
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Contact
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Department
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] View Comment
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] View Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] View Start ID
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] View End ID
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Range Comment
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Range Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Range Start ID
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Range End ID
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Created On
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Updated On
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns Infoblox VLAN records whose VLAN ID matches 200 .
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find infoblox 200 vlan
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Microsoft Graph Device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns Microsoft Graph devices known to Microsoft Graph's Active Directory Service
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find msgraph|microsoftgraph <hostname|domain_name> device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <hostname or domain_name> Yes ALL Hostname, Domain Name A full or partial hostname or domain name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Domain Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Manufacturer
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Platform
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Status
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device Category
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device Ownership
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device Version
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Profile Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Registration Date/Time
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Account Enabled
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] On Premises Last Synce Date/Time
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] On Premises Sync Enabled
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Created On
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Updated On
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns Active Directory computer records from Microsoft Graph whose Hostname matches corp-server
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find msgraph corp-server device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Microsoft Graph Managed Device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns Microsoft Graph devices known to Microsoft Graph's InTune service
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find msgraph <hostname> managed
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <hostname> Yes Text, MAC, Number Device Name A full or partial hostname
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device Name The hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Domain
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Manufacturer
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Edition
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Email
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] User
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] User Principal Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Ethernet MAC
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] WIFI MAC
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Subnet Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] IP Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Phone Number
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Notes
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device Category Display Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Sync Date/Time
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Free Storage Space (Bytes)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Total Storage Space (Bytes)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Physical Memory (Bytes)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Created On
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Updated On
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns InTune records from Microsoft Graph whose Hostname matches corp-server
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find msgraph corp-server managed
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Tenable Security Center
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all hosts known to scans in Tenable SecurityCenter. Results include its OS prediction & and various other metadata.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find tsc <subnet>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <subnet> No CIDR IP Address A network address in CIDR notation
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Security Server IP The IP Address used to collect on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Scan Name The reported Hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] IP Address
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Reverse DNS
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Prediction
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Prediction Confidence
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] System Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Total CVSs
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Scan Started At
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Scan Ended At
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find tsc 192.0.2.0/24 find tsc 192.0.2.3 find tsc Cisco\*
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Virtual Machines
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns information about virtual machines pulled from VMware and AWS.
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find virtualmachine|vm <ip|network|hostname>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP IP Addresses An IP Address of a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR IP Addresses A network address in CIDR notation that includes an IP Address of a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <hostname> Yes Text, Number, MAC Hostname A full or partial hostname
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hypervisor IP The IP Address of the Hypervisor (In the case of an AWS VPC, this is the network address of the CIDR Block assigned to the VPC)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname Hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Description The name given by the user to describe the VM
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Discovery Source The name of the collection job that discovered the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Power On Status The status of the VM
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor The vendor of the OS
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model This is the type of VM (For AWS this will be the Instance Type. For VMware this is just the VMware VM value)
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name Name of the OS
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version Version of the OS as derived from various properties
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version Full The full string used to derive the Name and Version
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Platform Architecture and other information relavant to what is running the VM
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] IP Addresses List of all the IP Addresses assigned to the VM
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] System Uptime (seconds) How long has the VM been running
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] System Time Current time for the VM
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] CPUs The number of CPUs assigned to the VM
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] CPU Cores The number of CPU Cores assigned to each CPU
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Threads Per Core The number of threads per core
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Tags A list of allt he user assigned tags
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Seen Time when the Vm was first seen
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen Time whent he VM was last updated
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all the virtual machines with a hostname that starts with corp
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find vm corp*
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Windows Management Instrumentation (WMI) Devices
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns data collected via the WMI collection type using the ITPIE Collection Engine (GUI or CLI).
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find wmi <ip|network|hostname>
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP IP Address The IP Address of a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR IP Address A network address in CIDR notation that includes the IP Address of a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <hostname> Yes Text, MAC, Number Device Name A full or partial hostname
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The IP Address used to collect on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The reported Hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Domain Name The reported Domain Name of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Vendor
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Platform
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Manufacturer Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Serial Number
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Part Number
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] SKU'
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] System Uptime
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] System Time
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Fingerprint
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Seen
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all devices whose Hostname matches corp-server
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find wmi corp-server
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Windows Management Instrumentation (WMI) Interfaces
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns Interface information about devices collected via the WMI collection type using the ITPIE Collection Engine (GUI or CLI).
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Syntax
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find wmi <ip|network|hostname|mac> interface
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Search Predicates
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Report Fields
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Option Supports Wildcard Predicate Type Matched Field Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <ip> No IP IP Address The IP Address of a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <network> No CIDR IP Address A network address in CIDR notation that includes the IP Address of a device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <hostname> Yes Text, Number Device Name A full or partial hostname
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] <mac> Yes MAC User A full or partial MAC
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Device IP The IP Address used to collect on the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Hostname The reported Hostname of the device
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Description
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Index
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] MAC
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Admin Status
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Oper Status
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Admin Speed
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Oper Speed
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Change
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] IP Addresses
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Vendor
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Model
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Name
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Vendor
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] OS Version
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Platform
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Manufacturer Type
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Last Seen
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] First Seen
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Examples
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] Returns all interfaces with a MAC that starts with aa:bb
[ITPIE:OPS Documentation | Intelligent Search | https://itpie-hostname/documentation/content/features/search-reference.html] find wmi aa:bb* interface
