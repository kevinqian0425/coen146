Kevin Qian

Overview

In this section, describe what you did in this lab and how you accomplished it.

# Sources

In this section, use all the resources you used, people not included

- Arman (because hes awesome)
- StackOverflow
- Beej's Guide to Computer Networking
- Python.org
- Google

# Questions

Type your answers to the following questions on a new line after each question.

If the current sequence number is 5, what should your sequence number be if the server received the incorrect checksum? What should it be if your
server received the correct checksum

If the incorrect checksum is received, the client needs to resend the message, thus the sequence number will still be 5. If the checksum is correct,
the next message can be sent which means the sequence number will be incremented to 6. 

How could we ensure the packets were delivered to the application in the correct order while allowing the client to not be blocked by a recvfrom call? (No code, just ideas). What sort of protcol could we use?

We can implement a sliding window protocol that uses the sequence number to arrange the order of the data. By using the sequence number, we can decide
if there is missing data that needs to be sent or resent.


What are some other ways besides checksums to check the correctness of packets?

Some other ways include multidimensional parity check that operates by arranging the message into a multidimensional grid and calculating a parity digit for each row and column or a cyclic redundancy check where blocks of data get a short check value attached, based on the remainder of a polynomial division of their contents

# Extra Credit Completion

Put an X in the following boxes if you completed the extra credits. Please describe your general process for doing this. What sorts of changes did you have to make in running your program?

[] Implement Go Back N Protocol for TCP and asynchronous

# Questions For TA

If you have any questions, just start typing them here. I gave you one to start off with. These arent necessary

1. Is this stuff actually ever used/ is it useful?

# Comments and Feedback

If you have anything youd like to tell me about, go ahead and write it in here. If its a GIF you want me to use or some thesis on why I suck, thats cool. Just remember that I control your grade for this lab.

