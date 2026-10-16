# Web Server

Source: ITPIE:OPS Documentation — Web Server
Source URL: https://itpie-hostname/documentation/content/administration/web-server.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Web Server
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] The Microsoft ASP.NET Core application uses the Kestrel web server to host several types of content:
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Server-side rendered views for certain sensitive workflows including login, logout, and licensing.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Public and private HTTP API endpoints, including an OpenAPI / Swagger API explorer when running in a Development environment.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] A bundled version of this documentation as a local static site.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] The single-page application (SPA) website.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Configuration
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] By default, the web server binds to all available IP addresses and listens on port 443 (HTTPS). The web server supports both HTTP/1.1 and HTTP/2 protocols. You may override the web server configuration in the application configuration file , depending on organizational policy.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Example of listening on specific interfaces and binding specific ports:
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] { "Urls": "https://127.0.0.1:443;https://[::1]:443" }
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Example of limiting maximum connections.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] { "Kestrel": { "Limits": { "MaxConcurrentConnections": 100, "MaxConcurrentUpgradedConnections": 100 } } }
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Example of limiting the HTTP protocol(s) served.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Warning
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Limiting the protocol may break integration with applications in ecosystems that do not have complete HTTP/2 support. For example, the popular Python library requests does not support HTTP/2.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Warning
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Some legacy load-balancers or proxies may not yet support HTTP/2.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] { "Kestrel": { "EndpointDefaults": { "Protocols": "Http2" } } }
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] SSL/TLS
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] The web server should be configured for HTTPS connections, secured with a trusted SSL certificate. An SSL certificate file and private key should be placed in the application configuration directory.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] /etc/itpie/ssl/itpie.crt /etc/itpie/ssl/itpie.key
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] These files should be in the PEM format (see RFC 7468 ). That is, the certificate file should start with this header:
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] -----BEGIN CERTIFICATE-----
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] And the key file should start with this header:
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] -----BEGIN PRIVATE KEY-----
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Since you are bringing these files, they may not have the correct permissions to be read by the itpie service user. Please set the correct permissions before starting the service. See the manual page for chmod(1) for more information.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] chmod (octal): 0640
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] chmod (symbolic): u=rw,g=r,o=
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Example of the Bash shell commands to set the correct permissions:
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] chown root:itpie /etc/itpie/ssl/itpie.* chmod 640 /etc/itpie/ssl/itpie.*
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] HTTPS policy
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] The application server enforces HTTP Strict Transport Security (HSTS).
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Tip
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] The Strict-Transport-Security header encodes the max-age value in whole seconds, but the ASP.NET Core configuration subsystem encodes the value as a TimeSpan string .
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] If you do not override the policy in application configuration, the defaults use a very short max-age (5 minutes), so as to not cause any problems if this is your first HSTS deployment.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] { "HttpsPolicy": { "Hsts": { "IncludeSubDomains": true, "MaxAge": "00:05:00" } } }
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] The defaults should produce the following header:
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Strict-Transport-Security: max-age=300; includeSubDomains
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] This policy should be overriden in application configuration. Industry experts recommend ramping up max-age in stages and testing thorougly before committing to a long max-age value.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Example final stage of the ramp, including a max-age of 365 days.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] { "HttpsPolicy": { "Hsts": { "IncludeSubDomains": true, "MaxAge": "365.00:00:00" } } }
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Content Security Policy (CSP)
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Warning
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Stable releases should not generate any policy violations. Detected violations may be bugs/regressions or an indication of a malicious actor exercising certain kinds of browser-based attacks.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] The application server implements a restrictive Content Security Policy (CSP) for each of the several subsites, depending on the technology in use. You can use the browser's developer tools to inspect document response headers.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Example of a Content-Security-Policy header:
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Content-Security-Policy: base-uri 'none'; connect-src 'self'; default-src 'none' 'report-sample'; frame-ancestors 'none'; font-src 'self'; form-action 'self'; img-src 'self'; style-src 'self'; report-uri /csp-reports
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] In addition to the client browser's developer tools console, policy violations should be reported to an application server endpoint and written to the service log . For reference, the Event IDs are as follows:
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] 204: Create violation report.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] 400: Create violation report failed.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Example:
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] warn: ITPIE.API.Security.ContentSecurity.ContentSecurityEndpoints.PostCspReport[204] [::1] 'user@example.com': Violation of script-src by 'eval' at https://itpie.example.com/. Source: https://itpie.example.com/main.js. Sample: `function eval() {`.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Antiforgery
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] The application server implements antiforgery protections against certain browser-based threats (CSRF/XSRF) using the default ASP.NET Core antiforgery subsystem.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] The technique is slightly different depending on the frontend technology in use, whther a browser or a JavaScript HTTP client, but always begins with the server generating a protected antiforgery cookie token per-user per-session.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Cookie: .AspNetCore.Antiforgery.<random-id>=CfDJ8AoE-...-LxXZLi8MuCE
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] The frontend must respond with the appropriate request token.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Server-side rendered forms, like the Login form, use a hidden form input: __RequestVerificationToken
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] The client SPA reads the request token cookie, XSRF-TOKEN , and sets the request token header, X-XSRF-TOKEN .
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] Any failure to validate the antiforgery token set will result in two messages written to the service logs, one by the Microsoft subsystem and one by the application server.
[ITPIE:OPS Documentation | Web Server | https://itpie-hostname/documentation/content/administration/web-server.html] warn: Microsoft.AspNetCore.Antiforgery.DefaultAntiforgery[4] The required antiforgery request token was not provided in either form field '__RequestVerificationToken' or header 'X-XSRF-TOKEN'.