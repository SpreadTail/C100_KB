# EXEC Modes

The Cisco Internetwork Operating System (IOS) utilizes a hierarchical command-line interface (CLI) to manage security and access control. Because unauthorized changes to network infrastructure can cause widespread service outages, the IOS restricts command availability based on the user's current "mode."

### User EXEC Mode
When an engineer first logs into a Cisco device, the system enters User EXEC mode. This is identified by the prompt `Router>`. This is the least privileged environment within the CLI. It allows the user to see limited, basic information about the device, such as system uptime, interface status, or basic connectivity tests like *ping*. In this mode, the user cannot modify any device settings or access sensitive configuration files.

### Privileged EXEC Mode
To gain access to more powerful diagnostic and management commands, the user must enter Privileged EXEC mode. This is accomplished by executing the `enable` command at the User EXEC prompt. Once entered, the prompt changes to `Router#`. 

Privileged EXEC mode provides access to advanced troubleshooting tools, such as debugging, system file management, and the ability to view the full configuration of the device. However, it is critical to understand the distinction in access levels: even in Privileged EXEC mode, the user remains in a read-only or diagnostic state. Neither User EXEC nor Privileged EXEC modes permit the user to make changes to the device’s operational configuration. Modifying the device requires moving into a higher-level Configuration mode, which is separated from these monitoring environments to prevent accidental changes.