# JavaScript communication

## WebSockets

### Protocol specification

WebSocket protocol is defined by [RFC-6455](https://tools.ietf.org/html/rfc6455)

#### On the wire

![WS Frame](https://github.com/ricardocasares/grow/blob/ricardocasares-js-communication/assets/ws-frame.png?raw=true "WS Frame")

A good explanation can be found on this talk [Inside WebSockets](https://www.youtube.com/watch?v=9FqjRN4VYUU)

##### FIN:  1 bit

Indicates that this is the final fragment in a message.  The first
fragment MAY also be the final fragment.

##### RSV1, RSV2, RSV3:  1 bit each

MUST be 0 unless an extension is negotiated that defines meanings
for non-zero values.  If a nonzero value is received and none of
the negotiated extensions defines the meaning of such a nonzero
value, the receiving endpoint MUST _Fail the WebSocket
Connection_.

##### Opcode:  4 bits

Defines the interpretation of the "Payload data".  If an unknown
opcode is received, the receiving endpoint MUST _Fail the
WebSocket Connection_.  The following values are defined.

*  %x0 denotes a continuation frame
*  %x1 denotes a text frame
*  %x2 denotes a binary frame
*  %x3-7 are reserved for further non-control frames
*  %x8 denotes a connection close
*  %x9 denotes a ping
*  %xA denotes a pong
*  %xB-F are reserved for further control frames

##### Mask:  1 bit

Defines whether the "Payload data" is masked.  If set to 1, a
masking key is present in masking-key, and this is used to unmask
the "Payload data" as per Section 5.3.  All frames sent from
client to server have this bit set to 1.

##### Payload length:  7 bits, 7+16 bits, or 7+64 bits

The length of the "Payload data", in bytes: if 0-125, that is the
payload length.  If 126, the following 2 bytes interpreted as a
16-bit unsigned integer are the payload length.  If 127, the
following 8 bytes interpreted as a 64-bit unsigned integer (the
most significant bit MUST be 0) are the payload length.  Multibyte
length quantities are expressed in network byte order.  Note that
in all cases, the minimal number of bytes MUST be used to encode
the length, for example, the length of a 124-byte-long string
can't be encoded as the sequence 126, 0, 124.  The payload length
is the length of the "Extension data" + the length of the
"Application data".  The length of the "Extension data" may be
zero, in which case the payload length is the length of the
"Application data".
