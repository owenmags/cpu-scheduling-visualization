# CPU Scheduling Visualization

### Operating Systems – Project 01

## Overview

This project is a simulation and visualization tool for various **CPU scheduling algorithms**, built as part of an Operating Systems course requirement. The goal is to help students and users understand how different CPU scheduling policies work by providing a visual representation of process executions, time calculations, and comparisons.

Developed with **Java (Terminal/console)** and **JavaScript HTML (GUI)** version.

---

## Scheduling Algorithms Implemented

1. **First Come First Serve (FCFS)** – Non-preemptive
2. **Shortest Job First (SJF)** – Non-preemptive
3. **Shortest Remaining Time First (SRTF)** – Preemptive
4. **Round Robin (RR)** – Preemptive with configurable time quantum
5. **Multilevel Feedback Queue (MLFQ)** – Preemptive, with 4 queues and configurable time quantums

---

## How to Run

### Web GUI

1. Open `index.html` in your browser.
2. Enter number of processes.
3. Fill in **Process ID**, **Arrival Time**, and **Burst Time**.
4. Select the desired scheduling algorithm.
5. Configure time quantum (for RR and MLFQ).
6. Click **Run Simulation**.

### Console Version (Java)

1. Open the Java project in NetBeans.
2. Run `Main.java` or `CPUSchedulingVisualization.java`.
3. Follow the prompts to:
   - Choose scheduling algorithm
   - Manually enter process data
   - View Gantt chart and performance metrics

---

## Output Features

- **Gantt Chart** (GUI-based)
- **Per-process metrics:**
  - Process ID
  - Arrival Time
  - Burst Time
  - Completion Time
  - Turnaround Time
  - Waiting Time
  - Response Time
- **Averages:**
  - Average Waiting Time
  - Average Turnaround Time

---

## Screenshots

### FCFS Simulation Example
![FCFS](https://github.com/user-attachments/assets/a1022cf0-dccd-402c-ace6-c0b6091d28a4)

### SJF Simulation Example
![SJF](https://github.com/user-attachments/assets/43449111-a0fa-4256-8319-c384e3e13c92)

### SRTF Simulation Example
![SRTF](https://github.com/user-attachments/assets/94d31548-9a6d-4bcb-9c38-d3181e0d1a5b)

### RR Simulation Example
![RR](https://github.com/user-attachments/assets/6a943ab8-54c0-492c-92d4-d58f5d522e26)
![RR Results](https://github.com/user-attachments/assets/b3699476-a890-4b7a-b9cb-924dd5fc44a1)

### MLFQ Simulation Example
![MLFQ](https://github.com/user-attachments/assets/0549ae90-89ae-4fa2-a815-e0213029dba5)
![MLFQ Results](https://github.com/user-attachments/assets/839c7d03-2b88-45f3-97c1-5772f27c1487)

---

## Sample Input

| Process | Arrival Time | Burst Time |
|---------|--------------|------------|
| P1      | 2            | 1          |
| P2      | 4            | 2          |
| P3      | 6            | 3          |
| P4      | 8            | 4          |
| P5      | 10           | 5          |

---

## Sample Output (FCFS)

### Gantt Chart:
| P1 | P2 | P3 | P4 | P5 |

### Metrics Table:

| PID | Arrival | Burst | Start | Finish | Waiting | Turnaround |
|-----|---------|-------|-------|--------|---------|------------|
| P1  | 2       | 1     | 2     | 3      | 0       | 1          |
| P2  | 4       | 2     | 4     | 6      | 0       | 2          |
| P3  | 6       | 3     | 6     | 9      | 0       | 3          |
| P4  | 8       | 4     | 9     | 13     | 1       | 5          |
| P5  | 10      | 5     | 13    | 18     | 3       | 8          |

Average Waiting Time: 0.80
Average Turnaround Time: 3.80

## Team Contributions

| Member                     | Roles & Responsibilities                                                                                                                                                                                              |
| -------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Pantine B. Hernando**    | - Led frontend design and implementation of Web GUI.<br>- Developed core backend logic for SRTF, RR, and MLFQ algorithms.<br>- Managed project structure and repository organization.                                      |
| **Owen Robert S. Magsayo** | - Contributed to Java backend development, including FCFS and SJF algorithms.<br>- Helped develop JavaScript logic in the Web GUI.<br>- Assisted in debugging and integration of frontend with backend. |

