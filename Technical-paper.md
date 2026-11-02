# The OSI Model

## Introduction

The Open Systems Interconnection (OSI) model explains how data travels between computers over a network. It was developed by the International Organization for Standardization (ISO) in the year 1970. This OSI model divides network communication into seven layers, and each layer has its own specific job. Because the layers are independent, engineers can design, test, and troubleshoot one layer without changing the others.

## The Seven Layers

1. **Physical Layer:** Sends raw bits over cables, fiber, or wireless signals. Examples are Ethernet cables and Wi-Fi radio signals.
2. **Data Link Layer:** Moves data between two devices on the same network using MAC addresses. Switches work at this layer.
3. **Network Layer:** Chooses the best path for data across different networks using IP addresses. Routers work at this layer.
4. **Transport Layer:** Delivers data between applications and controls reliability. TCP provides reliable data delivery with guarante, but UDP provides faster data delivery without guarantees.
5. **Session Layer:** Opens, manages, and closes the conversation between two applications.
6. **Presentation Layer:** Translates, encrypts, and compresses data so that both sides can understand it. TLS encryption and JPEG formatting are examples.
7. **Application Layer:** Provides network services directly to the user's software. HTTP, FTP, SMTP, and DNS belong here.

A simple way to remember the OSI model order from layer 1 to layer 1 by remembering the phrase "Please Do Not Throw Sausage Pizza Away".

## How Data Moves Through the Layers

When a user opens a website, the request starts at the Application layer. Each layer below it adds its own header information, which is called encapsulation. At the Physical layer, the data is sent as signals. The receiving computer reverses the process, and each layer removes its header until the web server receives the original request. This is called decapsulation.

## Why the OSI Model Is Useful

* It gives engineers a common language for discussing networks.
* It makes troubleshooting easier. For example, if a cable is unplugged, the problem is at layer 1. If an IP address is wrong, the problem is at layer 3.
* It allows products from different vendors to work together.

In practice, the internet runs on the simpler four-layer TCP/IP model. However, the OSI model is still widely used for learning and for diagnosing network problems.

## References

* [Cloudflare: What Is the OSI Model?](https://www.cloudflare.com/learning/ddos/glossary/open-systems-interconnection-model-osi/)
* [GeeksforGeeks: Open Systems Interconnection (OSI) Model](https://www.geeksforgeeks.org/open-systems-interconnection-model-osi/)
* [Wikipedia: OSI Model](https://en.wikipedia.org/wiki/OSI_model)
