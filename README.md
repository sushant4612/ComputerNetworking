# ComputerNetworking
## What is Computer Networking?

Computer networking refers to connected computing devices (such as laptops, desktops, servers, smartphones, and tablets) and an ever-expanding array of IoT devices (such as cameras, door locks, doorbells, refrigerators, audio/visual systems, thermostats, and various sensors) that communicate with one another.

## What is a Client?
A client is a computer hardware device or software that accesses a service made available by a server. The server is often (but not always) located on a separate physical computer.

## What is a Server?
A server is a physical computer dedicated to run services to serve the needs of other computers. Depending on the service that is running, it could be a file server, database server, home media server, print server, or web server.

## What is a Host?
A host is a computer, connected to other computers for which it provides data or services over a network. In theory, every computer connected to a network acts as a host to other peers on the network. In essence, a host reflects the logical relationship of two or more computers on a network.

To simplify this, suppose you want to download an image from another computer on your network. That computer is “hosting” the image and therefore, it is the host computer. On the other hand, if that same computer downloads an image from your computer, your computer becomes the host computer.

Your computer can be a host to other computers. Likewise, your router can be a host to other routers. But a host must have an assigned IP address. Therefore, modems, hubs, and switches are not considered hosts because they do not have assigned IP addresses.

## Bandwidth vs. Throughput vs. Latency

Bandwidth: This is about the volume of data that can be transferred over a network. The standard measurement for data transfer speed is megabits per second (Mbps).

Throughput: While bandwidth tells you how much data could theoretically be transferred across the network, throughput indicates how much data was actually transferred from a source at any given time.

Latency: This measures the time it takes for data to get its designation across the network. It is commonly measured as a round trip delay. Latency is usually measured in milliseconds(ms).


## Host vs Server
### Host:
A host can refer to any device that is connected to a network and that can send or receive data. It can be a computer, a smartphone, a tablet, or any other device that communicates over a network. In the context of networking, a host usually implies an endpoint device that can initiate or respond to communication requests within a network. For example, when you access a website from your computer, your computer is the host that's making a request to a server to retrieve the website's data.

### Server:
A server, on the other hand, is a type of computer or software that provides services or resources to other computers or devices on a network. Servers are designed to manage, store, send, and process data and requests. They are dedicated to providing specific functionalities or services, such as hosting websites, handling email, storing files, running applications, or managing network resources. Servers are built to be more robust, with higher performance and reliability to handle multiple requests from various clients or hosts simultaneously.

## Peer
![Link Name](Link URL)
- Host 1, Layer 5 is a peer to Host 2, Layer 5.
- Host 1, Layer 4 is a peer to Host 2, Layer 4.
- Host 1, Layer 3 is a peer to Host 2, Layer 3.
- Host 1, Layer 2 is a peer to Host 2, Layer 2.
- Host 1, Layer 1 is a peer to Host 2, Layer 1.
Note that it is commutative, so for example,

Host 2, Layer 5 is a peer to Host 1, Layer 5.
But to make sure you don't misunderstand, a peer is not always a layer. If I talk to you on a telephone, you and I are peers in that communication.

In the same telephone call, let's say they are mobile phones. The mobile phones each convert the audio to/from radio waves to a tower. In this case, the mobile phones are peers on the phone network.

However, in the same example, I am not a peer with your mobile phone because we are on different levels.

## Bandwidth vs. speed
The terms bandwidth and speed are often used interchangeably but not correctly. The cause of the confusion may be due, in part, to advertisements by internet service providers (ISPs) that conflate the two by referring to greater speeds when they truly mean bandwidth.

Essentially, speed refers to the rate at which data can be transmitted, while the definition of bandwidth is the capacity for that speed. To use the water metaphor again, speed refers to how quickly water can be pushed through a pipe; bandwidth refers to the quantity of water that can be moved through the pipe over a set time frame.

## Ping vs. Jitter
### Ping:
Definition: Ping is a network utility used to test the reachability of a host on an IP network. It measures the round-trip time for data to travel from one point to another and back. This utility sends an ICMP (Internet Control Message Protocol) echo request packet to a specific destination (such as a server or another device) and measures the time it takes for the echo reply packet to return. The time measured in milliseconds (ms) indicates the latency between the two points.

Example: If you're checking the ping to a gaming server, you might use the ping command in the Command Prompt or Terminal. For instance, typing "ping www.gamingserver.com" would send echo requests to that server, and you'd receive responses showing the time taken for each round trip. Let's say the output displays "Average = 25ms." This means the average round-trip time to that gaming server is 25 milliseconds.

### Jitter:
Definition: Jitter is the variation in the delay of received data packets traveling across a network. It measures the inconsistency in the latency, showcasing the fluctuations in the arrival time of data packets. Lower jitter values signify a more stable and consistent network connection, while higher jitter indicates irregularities in the arrival time of data packets.

Example: In a VoIP call (Voice over Internet Protocol), imagine you're communicating with someone over the internet:

Low Jitter Scenario: The voice data packets arrive at your device with minimal variation in their arrival times. For example, each packet consistently arrives at intervals of 20 milliseconds, maintaining a smooth and uninterrupted conversation.

High Jitter Scenario: The voice data packets arrive with irregular timing. Some packets might take 20 milliseconds to arrive, while others take 40 or 50 milliseconds. This irregular arrival causes disruptions in the conversation, leading to stuttering or out-of-sync audio due to the varied timing of the received packets.

## Packet
In networking, a packet is a small segment of a larger message. Data sent over computer networks*, such as the Internet, is divided into packets. These packets are then recombined by the computer or device that receives them.

*A network is a group of two or more connected computers. The Internet is a network of networks — multiple networks around the world that are all interconnected with each other.*

### What is a packet header?
A packet header is a "label" of sorts, which provides information about the packet’s contents, origin, and destination.

Packets consist of two portions: the header and the payload. The header contains information about the packet, such as its origin and destination IP addresses (an IP address is like a computer's mailing address). The payload is the actual data. Referring back to the photo example, the thousands of packets that make up the image each have a payload, and the payload carries a little piece of the image.

## Frame
In networking, a frame is a unit of data. A frame works to help identify data packets used in networking and telecommunications structures. Frames also help to determine how data receivers interpret a stream of data from a source

## Localhost:

Localhost is a networking term that refers to the loopback network interface of a device. It's used to access the network services that are running on the same device being used by the client. The loopback interface allows a computer to communicate with itself, meaning it can send and receive data internally without it ever leaving the device.

### Use Cases of Localhost:

Development and Testing: Developers often use localhost to test web applications or software locally on their machines without the need for an internet connection. It allows them to simulate a server environment on their own computer.

Server Testing: When setting up a server on a machine, developers or system administrators might use localhost to access server resources running on the same device for configuration and troubleshooting. This can include accessing databases, web servers, or any other server-based applications.

Isolated Environment: It provides a safe and controlled environment for testing new software or running local servers without affecting the actual network or other devices. It's an ideal way to try out new configurations or test potentially risky changes without impacting external systems.

Debugging: When troubleshooting networking or server-related issues, using localhost can help isolate whether problems are due to the network or external factors. It allows users to pinpoint issues that might be occurring within the local system itself.

Security and Privacy: Applications that run solely on localhost can offer a level of security and privacy, as they're not accessible from external networks. This could be advantageous for sensitive or developmental applications that shouldn't be accessible publicly.

## Noise
Noise refers to any external and unwanted information that interferes with a transmission signal. Noise can diminish transmission strength and disturb overall communication efficiency. In communications, noise can be created by radio waves, power lines, lightning and bad connections.

### Noise:
Noise refers to random and undesirable signals or interference that gets added to the original signal during transmission. It can degrade the quality of the transmitted data, making it difficult for the receiver to accurately interpret the intended information.

Example: In the context of a phone call, if you hear crackling, hissing, or other unwanted sounds while speaking to someone, that's noise affecting the audio signal. This noise could be due to electromagnetic interference, poor signal quality, or other environmental factors.

### Distortion:
Distortion occurs when the signal shape or quality is altered during transmission. It results in a modified or corrupted signal compared to the original, affecting the accuracy of the information being transmitted.

Example: When listening to music on a low-quality audio system, if the bass sounds muffled or the high notes are unclear, that's an example of distortion. The altered sound quality is due to the system's inability to faithfully reproduce the original signal.

### Attenuation:
Attenuation is the reduction in the strength or intensity of a signal as it travels through a medium or transmission system. It's a natural phenomenon where the signal weakens over distance or due to obstacles and other factors.

Example: In data communication over long-distance networks, such as fiber-optic cables or wireless transmissions, the signal strength diminishes as it traverses the medium. This loss in signal strength is attenuation. If a Wi-Fi signal weakens as you move farther away from the router, that's due to attenuation.

### Combined Effects:
These phenomena often occur simultaneously during signal transmission. For instance, as a signal travels over a long distance, it might suffer attenuation, leading to a weakened signal. Simultaneously, environmental interference or other factors could introduce noise, and the cumulative effect might cause distortion in the received signal, making the transmitted information less accurate or reliable.

In telecommunications and signal processing, mitigating these issues is crucial. Engineers use various techniques such as error correction codes, modulation schemes, shielding, signal amplification, and equalization to minimize noise, distortion, and attenuation, ensuring that the transmitted data is received as accurately as possible despite these challenges.

## Internet Vs Web
The internet is the vast global network of interconnected computers, enabling communication and data exchange. The web, short for World Wide Web, is a collection of interconnected documents and resources accessible via the internet through web browsers. In essence, the internet is the infrastructure, while the web is a service that operates on that infrastructure, allowing access to information and resources.
