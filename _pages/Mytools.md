---
layout: page
title: Tools & Projects
permalink: /tools/
description: "A collection of small tools, utilities, experimental applications, and personal software projects."
nav: true
nav_order: 6
---

## Tools & Projects

This page presents a collection of small tools, utilities, experimental applications, and personal software projects that I have developed for research, system monitoring, productivity, gaming, and other practical purposes.

Some projects are available as open-source software on GitHub.

---

## GPU Monitoring Tool

## GPU Server Monitor

**GPU Server Monitor** is a lightweight server monitoring application developed with **Streamlit** for monitoring the computing resources of our laboratory servers.

Our laboratory has multiple shared GPU servers that are used by students and researchers for deep learning experiments, medical image analysis, and other computational tasks. As the number of users increased, it became increasingly difficult to quickly understand which GPUs were available, which users were running jobs, and how long individual processes had been running.

To make GPU resource usage easier to understand, I developed this web-based monitoring tool.

### Main Features

The application collects and visualizes the current **CPU and GPU utilization** of laboratory servers. Resource usage is displayed using intuitive bar charts, allowing users to quickly identify available and heavily utilized computing resources.

In addition to overall resource utilization, the tool provides detailed information about individual processes running on each GPU, including:

- GPU utilization and memory usage;
- CPU utilization;
- running processes;
- the user associated with each process;
- process start time;
- detailed GPU usage for individual programs.

One of the most useful features is the ability to identify **who is currently using each GPU and when the corresponding process was started**. This makes it much easier for laboratory members to understand the current GPU allocation and coordinate the use of shared computing resources.

<div class="row justify-content-center mt-3">
  <div class="col-md-9 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/gpu-monitor.png" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
</div>

<div class="caption">
  GPU Server Monitor showing CPU and GPU utilization and detailed information about running processes.
</div>

### Practical Use in the Laboratory

The system is currently used in our laboratory, which has approximately **40 students and researchers**. Most laboratory members who use the shared computing servers regularly access the monitoring system to check GPU availability before starting experiments.

By providing a centralized overview of GPU usage, the tool reduces the need to manually connect to individual servers or ask other users about resource availability.

The tool has received positive feedback from laboratory members, particularly for its simple interface and the ability to quickly identify available GPUs and understand ongoing computational workloads.

### Implementation

The monitoring interface is implemented using **Streamlit**, enabling the system to provide an accessible web-based dashboard without requiring users to install additional client software.

The application is designed primarily for use within a shared laboratory computing environment.

- **Framework:** Streamlit
- **Purpose:** Shared CPU/GPU resource monitoring
- **Users:** Approximately 40 laboratory members
- **Source code:** [GitHub](YOUR_GITHUB_REPOSITORY_URL)

---

## Other Utilities

Additional small programs and experimental tools will be added here over time.
