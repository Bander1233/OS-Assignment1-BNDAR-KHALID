# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:A thread is a small unit of execution that runs inside a process and shares memory with other threads, whereas a process is an independent program with its own memory and system resources. In order to mimic CPU scheduling behavior, each process (P1–P10) in our assignment is represented by a thread.

Because threads have less cost during creation and context switching, they were employed in place of discrete processes. While threads enable effective execution inside the same application, creating several processes would need additional memory and system resources.

Additionally, because they share memory, threads communicate more quickly. Because numerous activities are carried out in a shared environment, they are perfect for replicating scheduling algorithms like Round-Robin.**

[Write your answer here. Consider: What is a process? What is a thread? How do they differ in terms of memory, resources, creation overhead? Why are threads more suitable for this simulation?]

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:A process is pushed back to the end of the ready queue in Round-Robin scheduling if it does not complete within the allotted time quantum. This prevents any one process from monopolizing the CPU and guarantees that every process has an equal opportunity to use it.**

[Write your answer here. Describe the specific behavior - where does the process go? When does it run again? Give an example from your actual program output showing a process that was re-queued.]

Example from my output:P1 completed quantum 3000ms │ Remaining time: 1773ms
P1 yields CPU for context switch
P1 (Priority: 3) added to ready queue
```
[Paste a relevant snippet from your program output here showing a process being re-queued]
```

**Explanation of example:In this example, process P1 did not finish execution within the time quantum (3000ms), so it yielded the CPU. The scheduler then re-added it to the end of the ready queue, allowing other processes like P2 and P3 to execute next.
This behavior ensures fairness and prevents starvation, which is a key goal of Round-Robin scheduling as explained in operating systems concepts.**
[Explain what's happening in the output snippet you pasted]

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:
New:
P1 is in the New state when the thread is created using new Thread(process) inside the addProcessToQueue method.
Runnable:
After the thread is added to the ready queue, it becomes Runnable, meaning it is ready to be executed by the CPU scheduler.
Running:
P1 enters the Running state when currentThread.start() is called. At this point, the CPU starts executing the process for its time quantum.
Waiting:
P1 enters the Waiting state when currentThread.join() is called in the main thread. The main thread waits until P1 finishes its execution for the current quantum.
Terminated:
P1 reaches the Terminated state when its remaining time becomes zero and it prints "finished execution!" in the output.**

[Write your answer here. For each state, explain when P1 enters that state during the simulation. Use your understanding of the code to trace through the lifecycle.]

1. **New**: [When is P1 in New state?]

2. **Runnable**: [When does P1 become Runnable?]

3. **Running**: [When is P1 Running?]

4. **Waiting**: [When/why would P1 be Waiting?]

5. **Terminated**: [When is P1 Terminated?]

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1: Web Server

**Description**:When loading webpages or responding to API queries, a web server manages several client requests concurrently. 
[Describe the real-world scenario or application]

**Why Round-Robin works well here**: By ensuring that every request receives an equal amount of CPU time, Round-Robin enhances responsiveness. When several users contact the server at once, it's crucial that no single request can block others.
[Explain why Round-Robin scheduling is suitable. Consider fairness, responsiveness, predictability, etc.]

### Example 2: Multimedia Systems (Media Player)
**Description**: Video playing, audio processing, and user interaction can all be handled concurrently by a media player.
[Describe the real-world scenario or application]

**Why Round-Robin works well here**: Round-Robin scheduling ensures smooth performance by giving each task a fixed time slice. This prevents lag and ensures that audio, video, and user interactions are processed fairly and continuously.
[Explain why Round-Robin scheduling is suitable. Consider fairness, responsiveness, predictability, etc.]

---

## Summary

**Key concepts I understood through these questions:**
1. The difference between threads and processes and why threads are more efficient
2. How Round-Robin scheduling ensures fairness using time quantum and re-queuing
3. The lifecycle of a thread and how it transitions between different states during execution

**Concepts I need to study more:**
1. Advanced thread synchronization techniques (e.g., locks and semaphores)
2. Other scheduling algorithms like Priority Scheduling and Shortest Job First (SJF)
