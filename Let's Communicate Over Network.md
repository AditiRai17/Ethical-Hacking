#### OSI MODEL describes seven layers that computer systems use to communicate over a network.

Let's Discuss

### OSI Model 

A multi-layered system that handles everything from the physical aspects of your devices and networks to how data is efficiently transported, checked, and presented in a way that your applications can understand.

1. Physical Layer (Layer 1): Manages the physical connection and raw data transmission. 
      Example :  Ethernet, USB, Fiber optic cables.
2. Data Link Layer (Layer 2): Handles data framing, error detection, and media access control. 
      Example : MAC addresses, Ethernet, Wi-Fi, Bluetooth.
3. Network Layer (Layer 3): Focuses on addressing, routing, and logical network topology. 
      Example : IP (Internet Protocol), Routing protocols (e.g., OSPF, BGP).
4. Transport Layer (Layer 4): Ensures reliable, end-to-end data transfer and manages flow control. 
      Example : TCP (Transmission Control Protocol), UDP (User Datagram Protocol).
5. Session Layer (Layer 5): Establishes, maintains, and terminates communication sessions. 
      Example : NetBIOS, RPC (Remote Procedure Call).
6. Presentation Layer (Layer 6): Deals with data translation, encryption, and data format conversion. 
      Example : SSL/TLS (Secure Sockets Layer/Transport Layer Security), JPEG, ASCII.
7. Application Layer (Layer 7): Provides user interfaces and network services for applications. 
      Example : HTTP, FTP (File Transfer Protocol), SMTP (Simple Mail Transfer Protocol).




#### Connection-Oriented 

Acknowledgement of receiving the data is sent from the server to the client ; Incase of data loss and error , the data is re-sent from client to the server
        
    Here's a step-by-step breakdown of how acknowledgments work in a TCP-based client-server communication:

        1. The client establishes a connection with the server through a process known as the three-way handshake.
        2. Once the connection is established, data is sent from the client to the server in the form of packets.
        3. For each received packet, the server sends an acknowledgment (ACK) back to the client, indicating the successful receipt of that packet.
        4. If the client doesn't receive an acknowledgment for a packet, it assumes that the packet may have been lost and retransmits it.
        5. This process continues until all data has been successfully received by the server.


#### Connectionless 

Client sends data to the server without expecting an Acknowledgement from the server i.e whether the data is received or not.

### IP (Internet Protocol): connectionless & unreliable

      - IP, or Internet Protocol, is like the postal system for the internet.
      - It's in charge of addressing and delivering data packets from one computer to another.
      - Just like how you put an address on an envelope to send a letter, IP assigns a unique address to each device on the internet. This address is called an IP address.

##### Example: 

Think of IP as the street address on a package you're sending through the mail.
If you want to send a package from your home to your friend's house, you need to put the correct addresses on it so the postal service knows where to deliver it.

### TCP (Transmission Control Protocol): connection-oriented & reliable

      1. TCP is like a reliable phone call. 
      2. It ensures that data sent from one computer to another arrives in the correct order and without errors. 
      3. If some data packets get lost or mixed up during transmission, TCP takes care of re-sending them. 
      4. It's a bit slower but very reliable, which makes it ideal for tasks like downloading files, sending emails, or browsing the web.


##### Example: 

Imagine you're having a conversation over the phone with a friend, and you want to make sure you both get every word in the right order. 
If your friend didn't hear something, they'd ask you to repeat it. This is similar to how TCP ensures all data is received correctly.

### UDP (User Datagram Protocol): connectionless & unreliable

      1. UDP is like sending a postcard. 
      2. It's faster and more lightweight than TCP but not as reliable.
      3. With UDP, you send data without confirming if it was received correctly. 
      4. It's great for real-time applications like online gaming, live video streaming, or voice calls where a small delay is acceptable, and you'd rather not wait for missing or out-of-order data to be retransmitted.

##### Example: 

Imagine you're sending a postcard to your friend while on vacation. 
You write a quick message and drop it in the mailbox, but you don't know if it arrives or if it's read in the right order. 
This is similar to how UDP works—quick and not worried about confirming receipt.

##### In summary, 

    IP gives devices their unique addresses on the internet, 
    TCP is like a careful and reliable phone call ensuring data arrives correctly, 
    and UDP is like a fast postcard delivery that doesn't worry too much about ensuring every piece of data arrives in order or at all. 

Each of these protocols has its own use cases depending on the needs of the application or service being used on the internet.



###### // Let's Discuss 3-Way Handshake in next blog //
