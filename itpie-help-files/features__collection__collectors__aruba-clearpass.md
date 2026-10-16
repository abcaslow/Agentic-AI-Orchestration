# Aruba ClearPass

Source: ITPIE:OPS Documentation — Aruba ClearPass
Source URL: https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Aruba ClearPass
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Collection Setup
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Step 1: Create an API Client in Aruba ClearPass
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Login to Aruba ClearPass
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Navigate to the Guest Manager using the top right hamburger menu and selecting "Guest"
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Inside the ClearPass Guest Manager navigate to “Administration” → “API Services” → “API Clients” and click Create API client
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] On the “Create API Client” form
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Add the “Client ID” (client user name)
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Set the “Operator Profile” to a “Profile” with the correct permissions
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Set the “Grant Type” to “Client credentials (grant_type=client_credentials)”
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Save the “Client Secret” key for later.
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Click "Create API Client" when finished.
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Step 2: Use Client ID and Secret Key to setup an Aruba ClearPass Credential in ITPIE
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Nagivate to Collection -> Credentials
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Click on "Create Credential"
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Change the Collector Type to ArubaClearPass
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Add your Client ID and Client Secret
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Click Add Credentials
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Step 3: Setup a collection job for the Aruba ClearPass server ip
[ITPIE:OPS Documentation | Aruba ClearPass | https://itpie-hostname/documentation/content/features/collection/collectors/aruba-clearpass.html] Add the Aruba ClearPass credential to a target with Collector Type set to ArubaClearPass