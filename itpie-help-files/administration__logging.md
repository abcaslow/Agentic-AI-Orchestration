# Logging

Source: ITPIE:OPS Documentation — Logging
Source URL: https://itpie-hostname/documentation/content/administration/logging.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Logging
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Tip
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] You should restart the service after any configuration changes.
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] The application server uses the Microsoft .NET logging subsystem to write messages to the the service log . You can configure the number and quality of the messages in the log in the application configuration file .
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Log level
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Every message is assigned a log level, which carries a meaning according to the table below. The log level can be used to filter the service log.
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] LogLevel Description
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Trace Contain the most detailed messages. These messages may contain sensitive app data. These messages are disabled by default and should not be enabled in production.
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Debug For debugging and development. Use with caution in production due to the high volume.
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Information Tracks the general flow of the app. May have long-term value.
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Warning For abnormal or unexpected events. Typically includes errors or conditions that don't cause the app to fail.
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Error For errors and exceptions that cannot be handled. These messages indicate a failure in the current operation or request, not an app-wide failure.
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Critical For failures that require immediate attention. Examples: data loss scenarios, out of disk space.
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] None Specifies that a logging category shouldn't write messages.
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Example of the default log level filter:
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] { "Logging": { "LogLevel": { "Default": "Information" } } }
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Log category
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Every message is assigned a log category, which is a semi-heirarchical dot ( . ) separated key. The specific or general log category can be used to filter the service log. The more specific or the longer the key, the higher the precedence of that configuration.
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Example of a super- and sub-category with differing log level filtering:
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] { "Logging": { "LogLevel": { "Default": "Information", "Microsoft": "Warning", "Microsoft.Hosting.Lifetime": "Information" } } }
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Log format
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] The logging subsystem and logging provider fill in several fields around the message template used at the point of logging.
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Timestamp: The timestamp of the log message being written, at seconds precision.
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Log Level: The log level of this message.
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Log Category: The log category is almost always mapped to a component's full name, including a namespace and class name (a dot '.' separated heirarchical name).
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Event ID: The event ID, if any, of this message, defaults to '0'.
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Message: The message, as provided by the component performing the logging at the point of logging.
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Example of the complete message template:
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] {Timestamp} {LogLevel}: {LogCategory}[{EventId}] {Timestamp} {Message}
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Example of the complete log message:
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] 2024-01-01 10:00:00 info: ITPIE.API.Example.ExampleController[0] 2024-01-01 10:00:00 An example log message.
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] You can configure log message formatting, to some degree.
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Log formatter
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] If you want log lines to not break after the source like normal, you can enable the ItpieSimple formatter. In the example below, the single line option is true , and a UTC timestamp in the provided format is added to each line.
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] Example of the custom simple log formatter:
[ITPIE:OPS Documentation | Logging | https://itpie-hostname/documentation/content/administration/logging.html] { "Logging": { "LogLevel": { "Default": "Information" }, "Console": { "FormatterName": "ItpieSimple", "FormatterOptions": { "SingleLine": true, "UseUtcTimestamp": true, "TimestampFormat": "HH:mm:ss " } } } }