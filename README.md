# REAL TIME SYSTEMS INTEGRATED LAB

# Feb 14 2019

1. Process Scheduling - Algorithms - Round Robin and Priority based scheduling of CPU tasks.

# March 21 2019 

2. Working with DESMO-J
3. Working with RTS algorithms in DESMO-J
4. Try SJF with DESMO-J for CPU Scheduling DESMO-J implementation change - TODO


Refactoring in DESMO-J for RTS environment.

DESMO-J 
1. Process
2. Process Example (main)
3. Processes
4. Task Generator


Process Example - init and doInitialSchedule method

# init - Process Example main - Queue property definition

    Probability methods-poisson,exponential,uniform for the queue.
    The incoming speed of tasks in queue.
   

    Poisson for incoming packets
    In consequtive packets - exponential distribution - delay 3 sec
    Packet arrival - uniform distribution ex every 7 sec or x sec

    Process execution time for initial stimulation time of tasks.

# doInitialSchedule - Process Example main
    
    Forked into two sub threads.
    
      pg.active -  Process Generator 
      cpu.active - cpu scheduler
     

# Process Queue -

    Packet/Task or even Truck - enters/leaves the queue.


# Task Generator -
    Generates task and it's pushed to queue

# Truck Generator -

    Constructor
    
    Lifecycle - while condition - endless execution 
    stimulation time in main function in minutes - after this time TaskGenerator ends.
    
# Task - 
   
    Constructor
    
    Lifecycle -
    
    idleQueue - Pushed when no task is waiting from CPU
    
    CPU queue check - for idle and if busy getFirst of active Process Queue
    
    Activate and hold - Timespan hold - arrival time hold - 1/lambda ( in consequitive in flow)
                                        cpu time hold packet arrival time hold
    
    When CPU is idle - idleQueue - 
    New process check - CPU in idleQueue? - activate CPU,passivate itself.
    FIFO scheduling.
    Changing the scheduling - change the CPU Scheduling (SJF) - unwind packets find one with least execution time.
    Task code changed to have mean Execution Time.
 
 #March 26 2019
 
 
 Scheduling based on Shortest Job First (SJF)
 
 Adding a new variable - priority - for Trucks and schedule based on priority 
 
 Scheduling based on Round Robin Scheduling
 
    
    
    
    
    
    
