# Reflection Questions

## Instructions
Answer the following questions about your learning experience. Each answer should be **at least 5-7 sentences** and show your understanding.

---

## Question 1: What did you learn about multithreading?

**Your Answer:** I gained an understanding of the basic principles of multithreading and how threads are utilized to mimic concurrent system operation through this project. I was aware of how Thread objects are used to generate threads and how the start() function is used to initiate them. Additionally, I learnt about the several thread states that exist during execution, including New, Runnable, Running, Waiting, and Terminated. The use of join() to alter execution order and synchronize threads is one key idea I learnt. I also came to understand how multithreading might enhance performance by facilitating the effective sharing of CPU time across several jobs. The ability of threads to mimic actual CPU scheduling behavior, such as Round-Robin, shocked me the most.

[Write your answer here. Discuss specific concepts like thread creation, thread states, how threads execute concurrently, what surprised you, etc.]

---

## Question 2: What was the most challenging part of this assignment?

**Your Answer:** Implementing the additional features, particularly the waiting time computation, was the most difficult aspect of this task. It was originally difficult to figure out just where to put the code inside the scheduler loop. Additionally, I had trouble accessing private variables like waitingTime and arrivalTime, which led to compilation issues. Because of this, I had to learn about encapsulation and the significance of getters and setters in object-oriented programming. Making sure the waiting time was accurately estimated without combining it with the execution time presented another difficulty. It required time to debug the logic and confirm it using the program's output. In general, the difficulty was both practical and intellectual.

[Describe the specific challenge. Was it understanding the code? Implementing a feature? Using Git? Explain what made it difficult and how it relates to the course concepts.]

---

## Question 3: How did you overcome the challenges you faced?

**Your Answer:** By breaking the difficulty down into smaller parts and concentrating on one aspect at a time, I was able to overcome the obstacles. To understand how the scheduler loop operates and where each action should be inserted, I thoroughly examined the code structure. I discovered how to correctly access private variables by using the getter and setter methods when I ran into problems with them. Additionally, I used debugging strategies such publishing intermediate values and contrasting predicted with actual outcomes. In order to further solidify my grasp of scheduling and threading principles, I also consulted the course materials and explanations. I was able to correct errors and enhance the code through methodical implementation and testing.

[Describe your problem-solving approach. Did you read documentation? Ask for help? Debug systematically? What resources did you use? What strategies worked?]

---

## Question 4: How can you apply multithreading concepts in real-world applications?

**Your Answer:**In practical applications, multithreading is frequently employed to enhance responsiveness and performance. Web browsers, for instance, employ many threads to load webpages, execute scripts, and process user input all at once. In a similar vein, mobile apps employ threads to carry out background operations, such as data downloads, without causing the user interface to freeze. Multithreading is used in games to simultaneously handle user interactions, physics computations, and visual rendering. I saw how threads mimic CPU scheduling in this assignment, which is comparable to how operating systems handle several tasks. Building effective and responsive software systems requires an understanding of multithreading.

[Give specific examples from real applications you use (web browsers, games, mobile apps, etc.). Explain why threads are useful in those scenarios. Connect to what you learned in this assignment.]

---

## Additional Reflections (Optional)

### What would you like to learn more about?
Advanced multithreading ideas like synchronization, mutex locks, and semaphores are things I'd like to learn more about. When several threads access shared resources, these ideas are crucial for preventing problems like race situations. Additionally, I'm curious to find out how operating systems identify and avoid deadlocks. I also want to delve more into alternative scheduling algorithms like Shortest Job First (SJF) and Priority Scheduling. My understanding of operating systems would increase if I could comprehend how these algorithms function in various situations. In general, I wish to improve my comprehension of thread management and concurrency.

[Any topics related to threading, concurrency, or operating systems that you're curious about?]

---

### How confident do you feel about multithreading concepts now?
I consider my comprehension of multithreading principles to be Intermediate. I am comfortable with fundamental ideas like thread creation, execution, and lifetime. I also comprehend the practical operation of scheduling algorithms such as Round-Robin. I still need additional experience, though, with more complex subjects like synchronization and securely managing shared data. I still don't fully understand several aspects, such thread communication and deadlocks. I think I can get more confident with additional practice and real-world experiences. All things considered, this job assisted me in laying a solid foundation.
[Rate yourself and explain: Beginner / Intermediate / Confident]

[Explain your rating - what do you understand well? What needs more practice?]

---

### Feedback on the assignment
Understanding the actual applications of operating systems ideas was greatly aided by this project. It made it possible for me to relate my academic understanding to practical code implementation. It was simpler to see how the system manages tasks thanks to the CPU scheduling simulation. But there were several difficult aspects of the task, particularly when it came to adding new features without explicit instructions. It could be simpler for pupils to do the assignments if there are additional examples or pointers. All things considered, the task was worthwhile and enhanced my comprehension of scheduling and multithreading.

[Any comments about the assignment? Was it helpful? Too easy/hard? Suggestions for improvement?]
