# Frequently Asked Questions

Source: ITPIE:OPS Documentation — Frequently Asked Questions
Source URL: https://itpie-hostname/documentation/content/faq.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Frequently Asked Questions | https://itpie-hostname/documentation/content/faq.html] Frequently Asked Questions
[ITPIE:OPS Documentation | Frequently Asked Questions | https://itpie-hostname/documentation/content/faq.html] Does ITPIE support 2FA using CAC, to log into Network Devices?
[ITPIE:OPS Documentation | Frequently Asked Questions | https://itpie-hostname/documentation/content/faq.html] ITPIE does not support CAC authentication.
[ITPIE:OPS Documentation | Frequently Asked Questions | https://itpie-hostname/documentation/content/faq.html] Since ITPIE is a persistent, server based application, it should be using a service account , not an individual user's account. Otherwise, ITPIE could only collect on devices if the user connects their CAC to a reader on the physical ITPIE server itself, in the datacenter. In the DoD, service accounts have an exemption from the CAC requirements.
[ITPIE:OPS Documentation | Frequently Asked Questions | https://itpie-hostname/documentation/content/faq.html] We also do not currently support SSH certificate based authentication.
[ITPIE:OPS Documentation | Frequently Asked Questions | https://itpie-hostname/documentation/content/faq.html] How does ITPIE handle Cisco ACI on the Nexus 9k?
[ITPIE:OPS Documentation | Frequently Asked Questions | https://itpie-hostname/documentation/content/faq.html] We don't have any special handling for Cisco ACI. Cisco ACI and Cisco APIC (cisco proprietary software) are tightly coupled. We can collect on the "underlay" network, for sure. We don't currently handle VXLAN for the "overlay" network. There are plans, to support some of the programmability aspects of NX-OS, such as RESTCONF, etc in the future.