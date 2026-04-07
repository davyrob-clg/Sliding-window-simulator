# UniGib TCP Sliding-Window-Protocol-Simulator

# Overview

The TCP sliding window protocol is a flow control mechanism that allows a sender to transmit multiple data packets (or bytes) before needing an acknowledgment (ACK), significantly improving network efficiency over "stop-and-wait" methods. It enables reliable, in-order delivery by managing a "window" of permitted packets, adjusting the amount of data in transit to avoid overwhelming the receiver.

# Key Aspects of the TCP Sliding Window:
* Window Size: Defines the number of bytes the sender can send before receiving an ACK.
* Dynamic Adjustment: The receiver notifies the sender of its available buffer space (receiver window) in its ACKs, allowing the sender to increase or decrease its sending rate dynamically.
* Flow Control: If the receiver's buffer fills up, it can shrink the window size (even to zero) to halt transmission, preventing buffer overflow.
* How it Slides: As the receiver acknowledges received data (ACK), the sender "slides" the window forward, permitting new segments to be transmitted.
* Sequence Numbers: Each byte is numbered to detect packet loss and reorder packets, ensuring reliable, ordered delivery. This protocol balances throughput and network load, making it crucial for modern network performance

# How does it work ?

We show three different protocols here

1.  Stop and Wait -the simplest and most inneficient
2.  The Go Back N - protocol
3.  The Selective Repeat protocol


Visit [here](https://sws.cs-unigib.org/)
