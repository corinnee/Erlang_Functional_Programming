# Erlang Message Passing System

## Project Description
This project is an Erlang-based concurrent message-passing system that consists of a logger, a consumer, and a buffer. It is designed to demonstrate the use of Erlang processes for handling messages, particularly in a multi-process environment. The system allows messages to be logged with sequence numbers, consumers to retrieve and process data from a shared buffer, and the buffer to manage data storage while notifying consumers about its status (empty, not empty, full). This program was completed for the 'Functional Programming' module at the University of Kent.

## Table of Contents
-[Key Components](#key-components)
-[Usage](#usage)

## Key Components
1. Logger: The logger is responsible for receiving messages and printing them with a sequence number to the console. It sequentially numbers each message it logs. It can be stopped upon receiving a specific "stop" message.

2. Consumer: The consumer is a process that interacts with the buffer. It checks whether the buffer is empty, waits if it is, and retrieves data from the buffer when it becomes non-empty. Once data is retrieved, it processes it and increments a counter. Consumers follow a state machine-like pattern with states c0, c1, c2, c3, and c4.

3. Buffer: The buffer acts as a shared storage space for data. It can receive data for storage, allow consumers to fetch data, and signal its status to consumers (empty, not empty, full) to control their behaviour. It also uses a state machine-like pattern with states c0, c1, c2, c3, and c4.

## Usage
To run the Erlang Message Passing System, follow these steps:

1. Ensure you have Erlang installed on your system.

2. Clone this repository to your local machine and navigate to the sub directory.

3. Compile the Erlang module by executing the following command in your terminal:

   ```shell
   erlc cb830.erl
   ```

4. Start an Erlang shell by running:
   ```shell
   erl
   ```
   
5. Start the main application by typing the following in the Erlang shell:
   ```erlang
     cb830:main().
   ```

The application will start, and you'll see messages logged to the console as the logger and consumer processes interact with the buffer.
