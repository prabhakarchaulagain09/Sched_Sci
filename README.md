# Sched\_Sci

A modular, adaptive Linux scheduling framework designed to optimize system performance across diverse workloads. This project integrates kernel-level scheduling, eBPF monitoring, workload classification, and experiment automation to evaluate and improve CPU, memory, and I/O performance.

## Overview
Modern systems often experience heterogeneous workloads, from CPU-intensive simulations to I/O-heavy databases. Traditional schedulers struggle to adapt dynamically, leading to suboptimal performance. 

This project aims to implement **workload-aware scheduling** by:
1. Monitoring system metrics in real-time using eBPF.
2. Classifying workloads based on observed patterns.
3. Dynamically selecting and switching optimal scheduling policies.
4. Providing a reproducible framework for experimentation and benchmarking.

---

## Key Features
- **Kernel-Level Schedulers** – CPU, memory, I/O, fairness-aware, and hybrid schedulers.
- **eBPF Monitoring** – Low-overhead real-time metric collection (CPU, memory, I/O).
- **Classification Engine** – Rule-based workload classification and policy selection.
- **Experiment Framework** – Automated scripts for reproducible testing across mixed workloads.
- **Benchmarks & Visualization** – Tools for comparing scheduler performance and generating graphs.

---

## Folder Structure
```text
workload-aware-scheduler/
├── docs/                  # Project documentation
├── kernel-schedulers/     # Kernel scheduler modules (Prabhakar)
├── ebpf-monitoring/       # eBPF programs and monitoring tools (Reedam)
├── classification-engine/ # Workload classification & policy selection (Bigyan)
├── experiment-framework/  # Automated experiments & reproducibility (Saniya)
├── benchmarks/            # Standard benchmark workloads
├── automation/            # Shared scripts for running experiments
├── visualization/         # Graphs and result visualization scripts
└── ci/                    # Continuous integration and basic build checks
```

## Folder Ownership
- kernel-schedulers/ – Prabhakar
- ebpf-monitoring/ – Reedam
- classification-engine/ – Bigyan
- experiment-framework/ – Saniya
- benchmarks/, automation/, visualization/ – Shared


