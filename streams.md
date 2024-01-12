# Streams

## Overview

- In this article, we will understand more about Streams, what they are, and why we need it.
- This article is for those who already heard about Streams when programming but have no idea about what is it and how it works.

## What is it?

- A Stream is a sequence of data elements made available over time. We can think that as a buffer of data that is either used to consume or produce data in small pieces.
- It's used to handle the continuous flow of data, allowing programs to read or write data piece by piece rather than loading the entire dataset into memory at once.
- Streams are commonly used for input and output operations, where data is processed or transmitted sequentially.

- ### Analogies to make it easier to understand

  - It serves as a pathway for the smooth flow of data, much like how a river stream transports water. The data moves through the stream, allowing for efficient processing and handling in various computational tasks.
  - Another way of thinking about it is that a stream is essentially like a pipe with a flow of water, where the water represents data and the pipe symbolizes the stream.

## Input Stream

- Handle the flow of data into a program. They are associated with data sources such as files, keyboards, network connections, or other input devices. Allow the program to read data from these sources.
- Operations for reading data.
- Used when a program needs to consume or process external data.

- ### Use cases

  - Reading data from a file, for example, a large video file that you need to perform a transformation and then write the transformed video to a new file.
  - Obtaining user input from various sources, like reading data entered by the user from the keyboard or a graphical user interface.
    - For example, in NodeJs we can process command-line inputs using streams provided by [Readline](https://nodejs.org/api/readline.html#class-interfaceconstructor) and [process.stdin](https://nodejs.org/api/process.html#processstdin).
  - Receiving data from a network, such as reading data from a socket when implementing network protocols.
  - Transforming raw data into a different format as it is read, for example, decoding binary data or converting character encodings.
    - It's particularly useful when the raw data needs to be processed or interpreted in a different form as it enters the program.

## Output Streams

- Manage the flow of data out of a program. They are associated with data destinations such as files, screens, or other output devices. Output streams enable the program to write data to these destinations.
- Operations for writing data.
- Used when a program needs to produce or send data to external locations.

- ### Use cases

  - Writing data to a file, such as storing the output of a program, or creating log/report files.
  - Displaying information to the user, through a command-line interface or a graphical user interface.
  - Sending data over a network, such as sending data to a server or another device through a network connection.
  - Serializing data structures and objects into a format suitable for storage or transmission, such as converting objects to JSON or XML before sending them.
    - When you want to save the state of an object, transmit structured data over a network, or store it in a format that can be easily reconstructed later.
    - Focused on preparing structured data for storage or transmission

## Duplex Streams

- A duplex stream can be thought of as a combination of both readable (input) and writable (output) streams. It provides a bidirectional flow of data, allowing components of a program to both consume and produce data simultaneously.
  - Both readable and writable streams are independent and each have separate internal buffer.
  - The reads and writes events happen independently.

- ### Use cases
  - Commonly used for sending and receiving data simultaneously, as seen in protocols like WebSockets.
    - WebSockets are specifically designed to enable realtime bidirectional communication between the server and client.
    - If you want to learn more about WebSockets read: [Ably WebSockets](https://ably.com/topic/websockets-vs-http).
  - Valuable in scenarios requiring continuous bidirectional data flow, such as chat applications or online gaming.
  - Duplex streams are often used to transform data during transmission. For example, data can be encrypted on the write side and decrypted on the read side, providing a secure communication channel.

## Disadvantages of streams

- Working with streams may introduce complexity to the code, especially for beginners.
- Error handling is more complex errors might occur at different stages of the stream, and handling them effectively requires a good understanding of the stream's lifecycle. Very different than debugging synchronous operations.
- In some cases, using streams might introduce a performance overhead compared to loading the entire dataset into memory, particularly for small datasets.
- Improperly managed streams can lead to resource leaks, such as unclosed streams, which may cause issues like file locks or network connection problems.
- In situations where the entire dataset can comfortably fit into memory, the added complexity of using streams may not be justified.

## References

- [Stack Overflow: Can you explain the concept of streams?](https://stackoverflow.com/questions/507747/can-you-explain-the-concept-of-streams)
- [Stack Overflow: NodeJS: What's the difference between a Duplex stream and a Transform stream?](https://stackoverflow.com/questions/18335499/nodejs-whats-the-difference-between-a-duplex-stream-and-a-transform-stream)
- [Cornell Computer Science](https://www.cs.cornell.edu/courses/cs312/2006sp/lectures/lec24.html)
- [Quora](https://www.quora.com/What-are-streams-in-programming)
- [Youtube - Streams Are Useful For - Intro to Parallel Programming - Udacity](https://www.youtube.com/watch?v=wYSNqRIoFrI)
- [Youtube - Advantage of Streams - Intro to Parallel Programming - Udacity](https://www.youtube.com/watch?v=sVMvohsYCQI)
- [Streams and how they fit into Node.js async nature.](https://levelup.gitconnected.com/streams-and-how-they-fit-into-node-js-async-nature-a08723055a67)

## Thanks for Reading!

- Feel free to reach out if you have any questions, feedback, or suggestions. Your engagement is appreciated!

## Contacts

- You can find this and more content on:
  - [GitHub](https://github.com/godinhojoao)
  - [LinkedIn](https://www.linkedin.com/in/joaogodinhoo/)
  - [Dev Community](https://dev.to/godinhojoao)

[Back to home](/readme.md)
