what is amqp?  
AMQP stands for Advanced Message Queuing Protocol. It's an open-standard application layer protocol for message-oriented middleware. In simpler terms, it's a way for different software components to communicate with each other by sending messages.  

AMQP defines a set of rules and formats for exchanging messages between different systems, making it easier for different software applications, written in different programming languages and running on different platforms, to communicate with each other reliably and efficiently.  

what it means? guest:guest@localhost:5672 , what is the first quest, and what is the second guest, and what is localhost:5672 is for?   
In the connection URL amqp://guest:guest@localhost:5672, each component serves a specific purpose:  
1. guest:guest: This part refers to the username and password used for authentication when connecting to the RabbitMQ message broker. In RabbitMQ, by default, there is a default user account with the username "guest" and password "guest". This is often used for testing or development purposes. In a production environment, it's advisable to use more secure credentials.  
2. localhost:5672: This part specifies the host and port of the RabbitMQ server. "localhost" indicates that the RabbitMQ server is running on the same machine as the code that's connecting to it. The port number 5672 is the default port for AMQP connections.  
So, when my code establishes a connection to amqp://guest:guest@localhost:5672, it's connecting to a RabbitMQ server running on the local machine using the default "guest" credentials for authentication.  