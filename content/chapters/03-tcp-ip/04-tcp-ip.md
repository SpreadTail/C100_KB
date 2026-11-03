# The TCP/IP Model

The **TCP/IP model** serves as the practical implementation framework for modern network communication. Originally developed by the **U.S. Department of Defense (DoD)**, this model describes the protocol suite that acts as the backbone of the Internet. The name is derived from its two foundational protocols: the **Transmission Control Protocol (TCP)**, which ensures reliable data delivery, and the **Internet Protocol (IP)**, which handles logical addressing and packet routing.

While the **OSI model** provides a conceptual roadmap for networking, the **TCP/IP model** represents the actual, functional implementation of those concepts. It streamlines the communication process into five layers, providing a more direct mapping of how software applications on a host interface with the physical hardware responsible for transmission. Each layer in this model encapsulates data and adds necessary control information as it travels down the stack to the physical medium, and then strips that information away as it moves up the stack at the destination.

The modular design of the **TCP/IP model** ensures that protocols at each layer can be updated or replaced without requiring changes to the entire architecture. This flexibility is what has allowed the Internet to evolve and scale while maintaining compatibility with diverse types of hardware and software.

The following table outlines the five layers of the TCP/IP model:

| Layer | Name | Primary Function |
| :--- | :--- | :--- |
| **5** | **Application** | Enables network services and user interaction with applications. |
| **4** | **Transport** | Manages end-to-end communication, reliability, and flow control. |
| **3** | **Network** | Handles logical addressing and routing of packets between networks. |
| **2** | **Data Link** | Manages physical addressing and transmission between adjacent nodes. |
| **1** | **Physical** | Transmits raw binary bits over the physical media (cables/wireless). |