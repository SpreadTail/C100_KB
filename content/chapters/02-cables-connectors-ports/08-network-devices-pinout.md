# Network Device Pinout Configurations

In 10BASE-T and 100BASE-TX networking, physical devices are manufactured with specific port wiring standards. These standards dictate which pins within the RJ45 interface are used for transmitting (Tx) and receiving (Rx) data. 

To ensure successful communication, these devices are split into two distinct categories based on their internal pin assignments. By default, a device configured with one pinout (e.g., sending on pins 1 and 2) must be connected to a device with the opposing pinout (e.g., receiving on pins 1 and 2). If two devices with the same pinout were connected directly, both would attempt to transmit on the same wires, resulting in no data transfer.

The following table categorizes common network devices by their standard pin assignments:

| Device Type | Transmit (Tx) Pins | Receive (Rx) Pins |
| :--- | :--- | :--- |
| **Computers** | 1 & 2 | 3 & 6 |
| **Routers** | 1 & 2 | 3 & 6 |
| **Routers** | 1 & 2 | 3 & 6 |
| **Switches** | 3 & 6 | 1 & 2 |

This configuration requires that connections between like-devices (e.g., Switch-to-Switch or Computer-to-Computer) be treated differently than connections between unlike-devices (e.g., Computer-to-Switch) to ensure the transmit pins of one device align with the receive pins of the other.