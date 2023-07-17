# ft_irc

This repository contains an IRC server implemented in C++98, adhering to the provided requirements. The IRC server is designed to handle multiple clients simultaneously, with non-blocking I/O operations using an equivalent of `poll()` (such as `select()`, `kqueue()`, or `epoll()`).

## Usage

To run the IRC server, follow these steps:

1. Clone this repository to your local machine:

   ```bash
   git clone <repository-url>
   cd ircserv
   ```

2. Compile the code using a C++98 compiler:

   ```bash
   make
   ```

3. Run the server with the specified port and password:

   ```bash
   ./ircserv <port> <password>
   ```

   Replace `<port>` with the port number on which the IRC server will listen for incoming connections, and `<password>` with the connection password required by IRC clients.

4. Connect to the server using IRSSI. Ensure that you use the correct server address, port, and password to establish a successful connection.

5. Use the IRC client to authenticate, set a nickname, a username, join channels, send and receive private messages, and perform channel-specific commands such as KICK, INVITE, TOPIC, and MODE.

Please note that this implementation focuses on the specified features and may not cover the full functionality of an official IRC server. The code has been written with an emphasis on cleanliness and adherence to C++98 standards.

## Notes

- The provided IRC server is designed to be compatible with a IRSSI. It supports user authentication, nickname and username setting, channel joining, private messaging, and channel-specific commands.

- Communication between the IRC client and the server is done via TCP/IP using the specified port number.

- The IRC server utilizes a non-blocking I/O mechanism to handle multiple clients simultaneously, ensuring the server never hangs.

- The server's code has been implemented in C++98, following the given requirements and restrictions.
