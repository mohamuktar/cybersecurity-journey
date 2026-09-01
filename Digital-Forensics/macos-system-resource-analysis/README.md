# macOS System Resource Analysis

## Context

Completed as part of my Cybersecurity Operations coursework at Highline College.

## Objective

Analyze CPU, memory, and disk activity using macOS Activity Monitor and investigate how operating system processes contribute to overall system performance.

---

## Environment

- Device: MacBook Air (2020)
- Processor: Apple M1
- Memory: 8 GB
- Operating System: macOS Tahoe 26.5.1

---

## Skills Practiced

- Operating system monitoring
- CPU utilization analysis
- Memory usage interpretation
- Disk activity analysis
- Background process investigation
- Technical research
- Performance troubleshooting

---

## Key Concepts Learned

### CPU

- Measured overall CPU utilization.
- Distinguished between User, System, and Idle CPU time.
- Observed how browser processes generate temporary CPU spikes.

### Memory

- Learned how memory pressure differs from total RAM usage.
- Investigated swap memory.
- Understood why 8 GB RAM becomes limiting during virtualization.

### Disk

- Observed background disk activity.
- Investigated FileVault and synchronization services.
- Learned that many operating system services continue working without direct user interaction.

---

## Research Highlights

During this lab I investigated several macOS system processes including:

- mdworker_shared
- kernel_task
- filevaultd
- contactsd
- recentsd

I learned the role each process plays within macOS and how legitimate system services can appear unfamiliar when first examining Activity Monitor.

---

## Reflection

One of the biggest takeaways from this lab was realizing how much activity occurs behind the scenes in a modern operating system. Before completing this assignment I assumed the computer was mostly idle when I wasn't actively using it. Instead, I discovered numerous background services responsible for indexing files, encrypting storage, synchronizing data, and managing system resources.

This exercise also highlighted the limitations of my current 8 GB MacBook Air for virtualization workloads. As I continue learning cybersecurity, especially using VMware Fusion and Kali Linux, upgrading to a system with additional memory will significantly improve my lab experience.

---

## Disclaimer

This repository summarizes my learning and reflections from coursework. It does not include copyrighted assignment instructions or assessment material.