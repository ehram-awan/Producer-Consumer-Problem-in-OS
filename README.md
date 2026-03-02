# Producer-Consumer Simulation in C++

This project demonstrates the **Producer-Consumer problem**, a classic synchronization problem in operating systems. It simulates the interaction between producer and consumer processes accessing a shared buffer. The project highlights both unsynchronized behavior (leading to race conditions) and a basic synchronized solution using simple mutual exclusion logic.

---

## Features

- **Problem Demonstration:** Shows the consequences of unsynchronized access to a shared buffer.
- **Synchronized Solution:** Implements basic synchronization to prevent race conditions, buffer overflow, and underflow.
- **Menu-Driven Interface:** Allows users to select between problem demonstration, solution, or exiting the program.
- **Interactive Simulation:** Users can produce and consume items step by step.

---

## Installation

1. Clone the repository:  
   git clone https://github.com/ehram-awan/producer-consumer.git

Navigate to the project folder:

cd producer-consumer

Compile the code with a C++ compiler:

g++ main.cpp -o ProducerConsumer

Run the program:

./ProducerConsumer   # Linux/Mac
ProducerConsumer.exe # Windows

---

## Usage

Launch the program.

Choose from the menu:

1. Demonstrate the Problem – Shows buffer issues without synchronization.

2. Provide the Solution – Demonstrates synchronized production and consumption.

3. Exit – Quit the program.

Follow prompts to produce or consume items.

Observe buffer behavior and any race conditions in the unsynchronized scenario.


---

## Methodology

Problem Demonstration: Users produce and consume items without synchronization, highlighting race conditions.

Solution Implementation: Uses basic mutual exclusion logic (mutex) and counters (full, empty) to simulate synchronized access.

Menu-Driven Approach: Allows users to select between unsynchronized demonstration and synchronized solution.


---

## Challenges

Understanding race conditions and buffer overflow/underflow issues.

Simulating basic synchronization without using advanced threading or semaphore constructs.

Ensuring correct user interaction and buffer updates.


---

## Limitations

No actual multithreading; synchronization is simulated.

Limited to a single buffer size (BUFFER_SIZE = 10).

Uses simple integer flags instead of real mutex/semaphore mechanisms.


---

## Future Enhancements

Implement true multithreading using std::thread and mutexes.

Replace simulated synchronization with semaphores for realistic thread safety.

Add dynamic buffer size and support for multiple producers and consumers.

Integrate logging for better visualization of buffer operations.


---

## Conclusion

This project provides a hands-on demonstration of the Producer-Consumer problem, emphasizing the importance of synchronization in shared resources. It serves as a foundation for understanding multithreading, race conditions, and synchronization mechanisms in operating systems.
