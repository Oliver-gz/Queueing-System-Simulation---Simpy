# Queueing System Simulation - Simpy

## About the Project
This project contains multiple basic examples about queueing system simulation for self-learning purpose. The simulations are realized with a Python package [Simpy](https://simpy.readthedocs.io/en/3.0/).

## Content Details
### 1 Simpy Basics
- Basic Concepts:
    - Example: simulate arrival times
- Events
  - Timeout Event
  - Generic Event
    - Example: for a single server queueing system, stop the system until 10 arrivals

### 2 Single Server Queueing System
- General Idea and Examples
  - Basic Example
  - Process N arrivals, get the expected time that an customer spends in the system
  - Stop system after N arrivals
  - stop system at time T
    - finish serving customers already in the queue (in the system)
    - get average time needed for serving remaining customers after system closed (this will decide when the server can g
    - finish the services already in progress and kick out customers in queue
    - stop system when N customers in the system, get the expected time
- Applications
  - check which event comes first, cancel event

### 3 Some Examples Before Multi-server Queue
- Print number of customers ahead of each customer
- Consider a special situation for the last example
- Yield a process

### 4 Multiple Server Queueing System
- Multi-server in Series (Servers can be different)
  - Basic Example
  - n series servers: we can create a list of servers
- Multi-server in Parallel (Identical Servers)
- Generalized Multi-server in parallel (different servers)
- Multi-server in parallel with multiple queues

### 5 Queueing System with Advanced Features
- Priority Resource
  - Process Interruption
      - Basic Example
      - Different kinds of interruptions: interrupt in service / interrupt in queue
      - After the interruption, the customer comes to the back of the queue
- Preemptive Resource
  - Basic example (not so reasonable): directly kicked off
  - More reasonable: go to the front of the line when getting kicked off from the service
