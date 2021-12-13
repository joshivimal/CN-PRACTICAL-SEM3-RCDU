# CN-PRACTICAL-SEM3-RCDU
This Repo is for our computer network practical of Sem-3 Ramanujan College, DU this consists of two Questions 
1.Simulate Cyclic Redundancy Check (CRC) error detection algorithm for noisy channel

CRC can detect all single-bit errors
CRC can detect all double-bit errors provided the divisor contains at least three logic 1’s.
CRC can detect any odd number of errors provided the divisor is a factor of x+1.
CRC can detect all burst error of length less than the degree of the polynomial.
CRC can detect most of the larger burst errors with a high probability.

2. Simulate and implement selective repeat sliding window protocol

Why Selective Repeat Protocol?
The go-back-n protocol works well if errors are less, but if the line is poor it wastes a lot of bandwidth on retransmitted frames. 
An alternative strategy, the selective repeat protocol, is to allow the receiver to accept and buffer the frames following a damaged or lost one.
Receiver must be able to accept packets out of order.
Since receiver must release packets to higher layer in order, the receiver must be able to buffer some packets.
Retransmission requests :

Implicit – The receiver acknowledges every good packet, packets that are not ACKed before a time-out are assumed lost or in error.Notice that this approach must 
be used to be sure that every packet is eventually received.
Explicit – An explicit NAK (selective reject) can request retransmission of just one packet. This approach can expedite the retransmission but is not 
strictly needed.
One or both approaches are used in practice.
Selective Repeat Protocol (SRP) :
This protocol(SRP) is mostly identical to GBN protocol, except that buffers are used and the receiver, and the sender, each maintains a window of size. 
SRP works better when the link is very unreliable. Because in this case, retransmission tends to happen more frequently, selectively retransmitting frames is more 
efficient than retransmitting all of them. SRP also requires full-duplex link. backward acknowledgments are also in progress.



