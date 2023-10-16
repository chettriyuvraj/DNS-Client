# Solution

## Opening a socket

- Lets have a look at the man pages for sockets, bind, et al first, pretty straightforward
- How do we implement system calls in Go? Went down a rabbit-hole of syscall (deprecated vs /x/sys). Decided to use /x/sys
- Let's read up a bit more about sockets quickly

### Sockets

- Abstraction to send and receive data across network
- Sockets are abstractions that encompass:
    - A given protocol
    - A given IP address
    - A given port
- The combination of these 3 things = socket address
- A socket is associated with a file descriptor, and have similar apis like read and write; but can do more things such as send and recieve 
- Sockets need not have a source socket address for simply sending data per se, however they need to be _bound_ to a source address to receive it
- Safe to say (?) sockets are an interface to be followed by end-user programs to deliver _messages_ to other programs via a protocol
