<ins> The OSI model </ins>

First of all ide like to go back to the TCP/IP modle in my previous document.

In the TCP/IP model theres 4 layers to it, Application, transport,network and physical.

The OSI Model is exactly that model however it involves being more intricate in some areas, if you have a look at the picture below you will see both models:

(Image of OSI and TCP/IP models)

You can see that the TCP/IP model is a much simpler version of the OSI model, however they are both models of communication.

As we did with the TCP/IP model i will break down the layers in the OSI model

Layer 7 - Application layer - Provides a service for the user

This layer is the start of the process in the OSI model. Just like the TCP/IP this layer is for human interaction.

For example a HTTPS website would be the application because thats what the user sees and can interact with therefore providing a service, It also identifies communication with partner and resource availability.

Layer 6 - Presentation layer - Translates, Encrypts and formats data

Why even have data if you cant read it? This is the layer just for that, it makes data thats sent to over the internet readable in plain text.
It also Encrypts and decrypts the data (through SSL/TLS), Converts the data format (encoding and decoding) and handles compression of data for transmission.

Layer 5 - Session layer - Creates sessions

Thats right, this layer does exactly what it says on the tin, This layer creates the session, Controls the dialog, maintains checkpoints and reconnection between the devices. This is used in NetBIOS, RPC and SQL sessions.

Layer 4 - Transport layer - gets the Data ready for transport to ensure fast and efficient delivery

This layer is where the data segmentation begins, it will split apart the data making it into smaller sizes (packets) for ease of transportation. It is also where TCP and UDP apply and ensures error recovery and end-to-end communication

Layer 3 - Network layer - Handles logical addressing and routing of packets

This layer determines the best route for the data to go to get to its destination, uses IP for routing packets, manages packet forwarding and supports layer 3 IP protocols (ICMP,IP)

Layer 2 - Data link layer - provides reliable node-to-node transfer

This layer uses MAC address for device identification, Performs error and correction (frame check sequence), Breaks down Packets into frames, manages access to the ethernet and switches.

Layer 1 - Physical layer - transmits the bits over a physical media

This layer turns the Data from being in frames to bit size pieces and the turns them back into packets once they have hit the destination intended.
It deals with some of the Network equipment that is able to transmit bits of data such as:

  - Cabling and media
  - Wireless Signals
  - Hardware Specs
  - Basic devices in the network - Hubs, repeaters and basic Network interface cards NICs
