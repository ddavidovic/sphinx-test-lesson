# Introduction

## History

- 1940-1960s: the first supercomputers
  - Military-driven evolution
  - First modern computers developed in WWII (ENIAC - Electronic Numerical Integrator and Computer)
  
```{figure} ../img/eniac.jpg
ENIAC in Philadelphia, Pennsylvania. Glen Beck (background) and Betty Snyder (foreground) program the ENIAC in building 328 at the Ballistic Research Laboratory (BRL). Figure taken from [Wikipedia](https://hr.wikipedia.org/wiki/ENIAC).
```

- Cold War: code breaking, intelligence gathering and processing, weapon design
  - ILLIAC-IV
    - Began in 1966; goal was 1 GFLOP/s; estimated cost $8 million
    - finished in 1972 at a cost of $31 million and a top speed below 1 GFLOP/s  
- 1975-1990: the Cray era
  - The speed was primarily achieved through two mechanisms:
    - vector processors
    - share memory multiprocessing
  - Believe that vector processors are better approach for HPC than using smaller processors. Saymour Cray once said: "If you were plowing a field, which would you rather use? Two strong oxen or 1024 chickens?"
- 1990-2010: the cluster era
  - Distributed memory computers emerged during 1980s
  - first cluster built in 1994 by Becker and Striling at NASA using available PCs and networking hardware (16 Intel 486DX PCs, 10 Mb/s Ethernet, 1 GFLOP/s) - named Beowulf
- 2010-present: the accelerator (GPU) and hybrid era
  - Increasing number of processor cores, not processor speeds
  - Development of GPUs and other accelerators
  - Today's supercomputers are hybrid clusters mixed of traditional processors and the accelerators

## Significance

## The roots of HPC in modern science
In modern science there are 3 methodologies: (staviti sliku umjesto list)
  1. Theory
  2. Experimentation
  3. Simulation

- When experimentation is very difficult or even impossible, for example in observing the macromolecular motions, assessing the efficiency of new drugs or describing fission reactions, the simulation can help people to test and prove their theories. Moreover, the simulations can better direct the experimentation phase.

- To keep pace with the scientific and industrial needs the simulations need to be more `accurate` and finish in less time which requires greater computing power

- Single processors cannot deliver that power
  - Making processor with higher clock speed is expensive and impossible due to the heat/power limitations
  - Expensive to put hugh memory on a single processor

```{callout} Solution
Parallel computing - split work into smaller pieces and divide it among numerous linked processors.
```

```{challenge} Challanges of parallel computing
Think of 3 possible challanges if you would have to split and process your work among several linked processors (computers).
```
---

## What is HPC?

**High Performance Computing (HPC)** refers to the practice of utilizing **very large computers** (supercomputers, clusters) to perform **computationally** and memory **intensive tasks** at **high speeds** using **parallel processing**.
HPC involves usage of advanced hardware and software to solve extremely complex problem that go beyond the capabilities of conventional computational systems.

<!--```{figure} ../img/HPC-map-2.png
:height: 12cm
Overview of HPC
```
-->

```{figure} ../img/HPC-map-3.png
:height: 12cm
Overview of HPC
```

<!--
## Parallel machine
```{figure} ../img/Fully-Connected-Network-Topology-diagram.png
Adapted from [Fully Connected Network Topology Diagram](https://www.conceptdraw.com/How-To-Guide/fully-connected-network-topology)
```
In HPC word, each computer in the network is called `compute node`.

- Definition of HPC + concept map
-->