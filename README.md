# Operating Systems - CPU Scheduling Algorithms

This repository contains implementations of various CPU Scheduling Algorithms, which are fundamental to understanding how operating systems manage process execution and resource allocation.

Currently, the repo features two primary non-preemptive scheduling strategies, with more algorithms (Preemptive SJF, Round Robin, Priority, etc.) planned for future updates.

## 📋 Implemented Algorithms
1. First-Come, First-Served (FCFS)
FCFS is the simplest scheduling algorithm. It executes processes in the exact order they arrive in the ready queue.

Type: Non-preemptive.

Characteristic: High average waiting time if a long process (convoy effect) arrives first.

Logic: The process that requests the CPU first gets the CPU allocated first.

2. Shortest Job First (SJF)
SJF selects the process with the smallest execution (burst) time to execute next.

Type: Non-preemptive (the current implementation).

Characteristic: Provides the minimum average waiting time for a given set of processes.

Logic: When the CPU is free, it is assigned to the process that has the smallest next CPU burst.

## 🛠️ Technical Details
Language: C / C++

Key Metrics Calculated:

Arrival Time (AT): Time at which the process arrives in the ready queue.

Burst Time (BT): Time required by the process for CPU execution.

Completion Time (CT): Time at which the process finishes execution.

Turnaround Time (TAT): Total Time Spent=CT−AT

Waiting Time (WT): TAT−BT

## 🚀 Upcoming Additions
[ ] Shortest Remaining Time First (SRTF) - Preemptive SJF

[ ] Round Robin (RR) Scheduling

[ ] Priority-Based Scheduling (Preemptive & Non-preemptive)

[ ] Multi-level Queue Scheduling

## 📂 How to Run
Clone the repository:
git clone https://github.com/lohotshreya/Operating-Systems.git

Navigate to the specific algorithm directory.
Compile using a C/C++ compiler (e.g., GCC):

gcc fcfs.c -o fcfs
./fcfs
