# Auto MDI-X

Auto MDI-X (Automatic Medium-Dependent Interface Crossover) is a feature implemented in modern networking hardware that eliminates the need for manual pin configuration. Historically, network engineers were required to manually select either a straight-through or crossover cable based on the specific types of devices being connected. If the wrong cable was used, the transmit (Tx) and receive (Rx) signals would not align, and communication would fail.

Auto MDI-X resolves this dependency by allowing a device to dynamically sense the signal on the wire and automatically configure its own port accordingly. When a link is established, the device detects whether the connected partner is transmitting on pins 1 and 2 or pins 3 and 6. The device then internally switches its own internal transmit and receive pathways to match the connection, ensuring that data is always sent to the partner’s receive pins and vice versa.

Due to the widespread implementation of this technology, physical crossover cables have become largely obsolete. Almost all modern network interface cards (NICs), switches, and routers support Auto MDI-X. This ensures that a standard straight-through cable will function correctly in any scenario, whether connecting a computer to a switch, or linking two switches together.
