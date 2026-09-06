# 🎫 Queue Line System – C++

A simple **Queue Line / Ticket Management System** built with **C++** to practice and demonstrate the practical use of **Queues, Stacks, Object-Oriented Programming, and basic data structures**.

The system simulates a real-world customer queue where clients receive tickets, wait for their turn, and are served in order.

## 📌 Project Overview

The `clsQueueLine` class manages a queue of customers using the **FIFO (First In, First Out)** principle.

Each customer receives a unique ticket containing:

* Ticket number
* Prefix
* Ticket issue time
* Number of waiting clients
* Expected serving time

The project also provides information about the queue and allows displaying tickets in different directions.

## ✨ Features

* 🎫 Issue new customer tickets
* 🔢 Generate unique ticket numbers
* 🕐 Record ticket issue time
* 👥 Track waiting clients
* ⏱️ Calculate expected serving time
* 👤 Serve the next customer
* 📊 Display queue information
* ➡️ Display tickets from first to last
* ⬅️ Display tickets in reverse order
* 📋 Display all ticket details
* 🧱 Practice nested classes and OOP concepts
* 📚 Practical use of `Queue` and `Stack`

## 🧠 Data Structures Used

### Queue

The main queue follows the FIFO principle:

```text
First Client → Second Client → Third Client
     ↑
   Served
```

The first client who receives a ticket is the first client to be served.

### Stack

A temporary stack is used when displaying the queue in reverse order without modifying the original queue.

## 🏗️ Main Class

### `clsQueueLine`

Responsible for managing the entire queue.

Main operations include:

```cpp
IssueTicket()
WaitingClients()
WhoIsNext()
ServeNextClient()
ServedClients()
PrintInfo()
PrintTicketsLineRTL()
PrintTicketsLineLTR()
PrintAllTickets()
```

## 🎟️ Ticket System

Each ticket is represented by the nested `clsTicket` class.

A ticket contains:

```text
Prefix
Ticket Number
Ticket Time
Waiting Clients
Average Serve Time
Expected Serve Time
```

The full ticket number is generated using:

```text
Prefix + Ticket Number
```

For example:

```text
A1
A2
A3
```

## ⏱️ Expected Serving Time

The expected serving time is calculated based on:

```text
Average Serve Time × Waiting Clients
```

For example, if the average serving time is 5 minutes and there are 3 waiting clients:

```text
Expected Serve Time = 5 × 3 = 15 Minutes
```

## 🖥️ Example

A queue might look like:

```text
Tickets: A1 <-- A2 <-- A3 <--
```

After serving the first client:

```text
Tickets: A2 <-- A3 <--
```

And the next client would be:

```text
A2
```

## 🛠️ Technologies

* **C++**
* Object-Oriented Programming (OOP)
* STL `queue`
* STL `stack`
* Classes & Nested Classes
* Basic Date & Time Handling

## 🎯 Learning Objectives

This project was built to strengthen my understanding of:

* Queue data structures
* Stack data structures
* FIFO behavior
* Working with STL containers
* Object-Oriented Programming
* Encapsulation
* Nested classes
* Managing objects inside data structures
* Simulating real-world systems using programming concepts

## 📂 Project Structure

```text
Queue-Line-System/
│
├── clsQueueLine.h
├── clsDate.h
└── main.cpp
```

> The exact file structure may vary depending on the implementation.

## 🚀 Future Improvements

Possible improvements for future versions:

* Add a graphical user interface
* Add multiple service counters
* Support different queue types
* Store ticket history
* Add ticket cancellation
* Save queue data to a file or database
* Add estimated waiting time for each customer
* Improve ticket and queue management

## 👨‍💻 About the Project

This project is part of my journey in learning **C++ and Data Structures**, with a focus on understanding how common data structures can be applied to build practical systems.

> **From data structures to real-world applications. 🚀**
