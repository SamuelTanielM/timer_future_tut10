# timer_future_tut10

Nama: Samuel Taniel Mulyadi
NPM : 2206081805

**Experiment 1.2: Understanding how it works.**
![Experiment 1.2: Understanding how it works. capture1.2 .png](images/capture1.2.png)

The output "Samuel's Komputer: hey hey" is printed before the task is spawned because it's part of the main function and executed immediately. Then, the task is spawned asynchronously to print "Samuel's Komputer: howdy!" and wait for the timer future to complete, which is 2 seconds. 

The execution of the spawned task and the main function runs concurrently, but the main function doesn't wait for the spawned task to complete. This is why "howdy!" and "done!" are printed in between the initial and final print statements, meanwhile the main function which print "hey hey" immediately printed first.

In essence, the asynchronous nature of spawning tasks allows the main function to continue its execution while the spawned task operates independently. Thus, the order of printing reflects the concurrent execution of tasks rather than a sequential flow.
