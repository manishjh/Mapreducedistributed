1. Your job is to implement a distributed MapReduce.
2. consisting of two programs, the master and the worker.
3. There will be just one master process, and one or more worker processes executing in parallel. 
4. In a real system the workers would run on a bunch of different machines, but for this lab you'll run them all on a single machine. (docker)
5. The workers will talk to the master via RPC.
6. Each worker process will ask the master for a task, read the task's input from one or more files, execute the task, and write the task's output to one or more files. 
7. The master should notice if a worker hasn't completed its task in a reasonable amount of time (for this lab, use ten seconds), and give the same task to a different worker.