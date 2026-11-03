# The OSI Model

The **Open Systems Interconnection (OSI) model** is the industry-standard conceptual framework for network communication. Developed by the **International Organization for Standardization (ISO)**, it serves as a universal roadmap that defines how data moves from one device to another. By establishing this model, the ISO created a common language that allows diverse systems, regardless of their manufacturer or internal architecture, to communicate effectively.

The **OSI model** is organized into seven distinct layers. This hierarchical structure is designed to break down the highly complex process of data transmission into manageable, functional segments. Each layer performs specific tasks, such as addressing, routing, or error checking, and provides services to the layer directly above it. This modularity is a critical feature of the model: it allows engineers to troubleshoot connectivity issues within a specific layer without needing to reconfigure the entire stack, and it enables different technologies to interact seamlessly as long as they adhere to the standard definitions at each layer.

The following table outlines the seven layers of the OSI model, listed from the top (closest to the user) to the bottom (closest to the physical media):

| Layer | Name | Primary Function |
| :--- | :--- | :--- |
| **7** | **Application** | Provides network services directly to the user's software. |
| **6** | **Presentation** | Handles data formatting, encryption, and compression. |
| **5** | **Session** | Manages, maintains, and terminates connections between applications. |
| **4** | **Transport** | Ensures reliable data delivery and flow control. |
| **3** | **Network** | Determines logical addressing and the path (routing) for data. |
| **2** | **Data Link** | Packages data into frames and manages physical addressing. |
| **1** | **Physical** | Transmits raw binary bits over the physical communication media. |