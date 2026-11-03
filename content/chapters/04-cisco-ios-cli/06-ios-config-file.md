# Cisco IOS Configuration Files

The Cisco Internetwork Operating System (IOS) utilizes two distinct text files to manage device configurations: the **running-configuration** and the **startup-configuration**. These files serve different purposes, separating the device's active operational state from its stored, persistent settings.

### The Running Configuration
The `running-config` file dictates the current operations of the device. It is stored in the device's Random Access Memory (RAM), meaning it contains all settings currently in effect. Because RAM is volatile, the `running-config` is transient, any modifications made to this file take effect immediately, but they will be permanently lost if the device is powered off or restarted. Administrators can verify the current active configuration at any time by executing the command `show running-config`.

### The Startup Configuration
The `startup-config` file is stored in the device's non-volatile memory (NVRAM). This file acts as the persistent storage for the device. During the boot process, the device initializes by copying the contents of the `startup-config` into the `running-config` file in RAM, establishing the operating environment. Users can inspect the saved settings by using the `show startup-config` command.

### Persistence of Changes
Because changes applied to the `running-config` are lost upon reboot, administrators must explicitly save their work to ensure it persists. This involves copying the `running-config` to the `startup-config`. By performing this save operation, the current configuration is written to the NVRAM, guaranteeing that the settings will be reloaded the next time the device starts.

### Saving and Resetting Cisco Configurations

To maintain configuration persistence, it is necessary to transfer the active settings from volatile RAM to non-volatile memory (NVRAM). This ensures that the device’s operational parameters remain intact following a power cycle or system restart. In Privileged EXEC mode, several commands are available to commit these changes. The standard, recommended method is the `copy running-config startup-config` command. Legacy commands such as `write` or `write memory` are also supported and functionally identical, they all trigger the process of overwriting the stored `startup-config` file with the current `running-config`.

In scenarios where a device must be returned to its original factory state—such as during equipment decommissioning or when a clean reconfiguration is required—the administrator must clear the persistent configuration. This is a destructive process that removes all custom settings, including passwords, interface configurations, and routing protocols.

To perform a factory reset, the `startup-config` file must be deleted from NVRAM. This is typically achieved using the `erase startup-config` command. Depending on the IOS version and device model, alternative commands such as `write erase` or `erase nvram` may also be utilized to accomplish this task. It is critical to understand that erasing the `startup-config` file does not immediately remove the current operational configuration from RAM. The device will continue to function with its existing settings until it is rebooted. Therefore, after erasing the configuration, the administrator must issue the `reload` command. Upon restart, the device will detect the absence of a `startup-config` file and initialize using its default factory settings.