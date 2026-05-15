---
layout: post
title: HPC Power Overload Handling Framework
subtitle: Graduate Research, University of Texas at Arlington
tags:
  - Python
  - Socket.IO
  - Slurm
  - OpenMP/MPI
  - Bash/Shell
published: true
---

**My Role:** _Graduate Research Assistant_

**Tech Stack:** _Python, Slurm, Socket.IO, Bash/Shell Scripting, OpenMP/MPI_

**Platform:** _Linux-based HPC Cluster_

Developed a Python-based framework for detecting and mitigating power overload events in **HPC clusters**. The framework integrates with the **Slurm** job scheduler to monitor active workloads and collects real-time power telemetry from an external **PDU**. When an overload is detected, the system coordinates a distributed client-server bidding mechanism to emulate interactions between the HPC manager and users, then applies **CPU-frequency scaling** across the cluster to reduce power consumption.

The framework also includes rollback logic to restore normal CPU-frequency settings once the overload condition is resolved. This allowed the system to respond dynamically to overload events while minimizing unnecessary disruption to running **OpenMP/MPI** workloads.

![MPR](/assets/img/pdu_events_plot.png)
