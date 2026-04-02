# Development Log

## Instructions
Document your development process as you work on the assignment. Add entries showing:
- What you worked on
- Problems you encountered
- How you solved them
- Time spent

**Requirements**: Minimum 5 entries showing progression over time.

---

## Example Entry Format:

### Entry 1 - [April 1, 2026, 2:30 PM]
**What I did**: Forked the repository and set up my student ID

**Details**: 
- Created GitHub account with university email
- Forked the starter repository
- Changed student ID on line 92 to my actual ID (441234567)
- Compiled and ran the program successfully

**Challenges**: Had to install JDK first because javac wasn't recognized

**Solution**: Downloaded JDK 17 from Oracle website and set PATH variable

**Time spent**: 30 minutes

---

## Your Development Log:

### Entry 1 - [mar 28, 2026, 10:26 PM]
**What I did**:Configure the project and execute the first code. 

**Details**:opened Visual Studio Code and started the project.
examined the classes (Process, SchedulerSimulation) and code structure.
The student ID in the main output area was updated.
successfully compiled and executed the application to comprehend the fundamental behavior 

**Challenges**:I was initially unfamiliar with the scheduler simulation's operation. 

**Solution**:Go over the code carefully and see the results step-by-step. 

**Time spent**:40 minutes 

---

### Entry 2 - [mar 30, 2026, 11:26 AM]
**What I did**:Implemented Feature 1 (Process Priority) 

**Details**: The Process class now has a priority property.
Priority was added to the constructor.
Random priority values (1–5) were generated.
When adding processes to the queue, the output was updated to show priority.

**Challenges**: Knowing where to set the priority without causing code errors

**Solution**: added the value at process creation and tracked object creation in main().

**Time spent**: 50 minutes

---

### Entry 3 - [mar 30, 2026, 10:26 PM]
**What I did**:Implemented Feature 2 (Context Switch Counter) 

**Details**: A static counter variable was added.
increased it each time a process began to run.
Total context shifts were printed at the program's conclusion.

**Challenges**:Choosing where the counter should be increased 

**Solution**:put it ahead of the current thread.start() within the scheduler loop 

**Time spent**:35 minutes 

---

### Entry 4 - [Apr 1, 2026, 9:02 PM]
**What I did**: Implemented Feature 3 (Waiting Time Tracking)

**Details**: ArrivalTime and WaitingTime variables were added.
utilized the system.To monitor execution time, use currentTimeMillis().
Waiting time was computed using startArrival time
After every execution, the arrival time was updated.

**Challenges**: Errors were found in private variables.

**Solution**: Used getter and setter methods to access and update values correctly

**Time spent**: 1 hour

---

### Entry 5 - [Apr 1, 2026, 10:15 PM]
**What I did**:Tested and debugged the full program 

**Details**: ran the simulation several times.
Verified output accuracy (waiting time, execution order, queue behavior)
corrected duplicate items and made sure the summary table was accurate.

**Challenges**: In the output, a few values were duplicated.

**Solution**: Loop logic was reviewed, and each procedure was accurately printed once.

**Time spent**: 45 minutes

---

### Entry 6 - [Optional - Apr 2, 2026, 5:15 PM]
**What I did**: Completed documentation (ANSWERS & REFLECTION)

**Details**: All conceptual questions were addressed.
Connected responses to the code and real output
wrote a reflection based on what I had learned.

**Challenges**: Writing clear academic answers in English

**Solution**: Structured answers using course concepts and examples from output

**Time spent**: 2 hour and 30 minutes

---

## Summary

**Total time spent on assignment**: [7 hours]

**Most challenging part**:Implementing the waiting time feature and precisely positioning the code inside the scheduler loop proved to be the most difficult portion. Timing logic and thread execution sequence have to be understood. 

**Most interesting learning**: Seeing Round-Robin scheduling in action and how threads mimic actual CPU activity was the most fascinating aspect.

**What I would do differently next time**: The next time, rather than waiting until the very end, I would design the features in advance and test each component right away after implementation.
