# Reverse-engineer malware → YARA/Sigma rule

## Objective

Designed and implemented a controlled cybersecurity lab environment to simulate and analyze cyber attack scenarios. Configured log ingestion and monitoring within a Security Information and Event Management (SIEM) platform to detect and investigate security events. Generated test telemetry to emulate real-world attack techniques, enhancing practical knowledge of threat detection, network security, attack methodologies, and incident response processes.

### Skills Learned

- Advanced understanding of SIEM concepts and practical application.
- Proficiency in analyzing and interpreting network logs.
- Ability to generate and recognize attack signatures and patterns.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used

- Security Information and Event Management (SIEM) system for log ingestion and analysis.
- Network analysis tools (such as Wireshark) for capturing and examining network traffic.
- Telemetry generation tools to create realistic network traffic and attack scenarios.

## Steps

Assembly language represents the lowest level of the software execution chain. Even when source code is unavailable, various analysis and disassembly tools can translate compiled programs into assembly instructions. Every statement written in a high-level programming language is ultimately converted into one or more assembly instructions that the processor can execute.

From a reverse engineering perspective, assembly code provides a direct view of how software operates. Since all program logic must eventually be expressed through assembly instructions, understanding assembly language is essential for analyzing and reversing software behavior.

There is no single universal assembly language. Different processor architectures use different instruction sets, such as:

x86 (32-bit)
x64 (64-bit)
ARM
PowerPC (PPC)

To become proficient in reverse engineering, it is necessary to understand the assembly language of the target platform. This project focuses on analyzing and understanding assembly instructions across the x86, x64, and ARM architectures, which are among the most widely used processor platforms in modern computing systems.

<img width="740" height="399" alt="image" src="https://github.com/user-attachments/assets/6c5a0d3e-c3dc-4ce7-a1fb-ce8f7262a4f0" />

Code-level reverse engineering involves analyzing machine code to identify and reconstruct the underlying software logic, algorithms, and design concepts. The primary objective is to understand how a program functions when the original source code is unavailable.

Successful reverse engineering requires a strong understanding of several fundamental areas, including:

CPU Architecture and Instruction Execution
Operating System Internals
Memory Management
Software Development Processes
Program Execution Flow

By combining knowledge from these domains, analysts can interpret machine-level instructions and translate them into meaningful representations of the original software behavior.

To support the reverse engineering process, a variety of specialized tools are commonly used, including:

IDA Pro – Advanced disassembler and debugger for static code analysis.
Ghidra – Open-source reverse engineering suite developed by the NSA.
OllyDbg – Dynamic debugger widely used for Windows application analysis.
SoftICE – Low-level system debugger for kernel and application debugging.
Additional Analysis Tools – Various utilities for disassembly, debugging, binary inspection, and malware analysis.

<img width="740" height="435" alt="image" src="https://github.com/user-attachments/assets/3e84a8da-0318-4ced-b47f-0430489541f2" />

System-level reverse engineering focuses on analyzing software behavior during execution by collecting information from the operating system and monitoring the interactions between the application and system resources. Unlike code-level reverse engineering, which examines machine code and program logic, system-level reverse engineering emphasizes understanding how a program behaves in a live environment.

This approach involves:

Inspecting executable files and their properties.
Monitoring process creation and termination.
Tracking file system activities.
Observing registry modifications.
Analyzing network communications.
Monitoring input and output operations.
Examining interactions between the application and the operating system.

A significant portion of this information is obtained through operating system monitoring and analysis tools, which provide insights into the software's runtime behavior and system impact.

Commonly used tools for system-level reverse engineering include:

Sysinternals Suite – A collection of advanced Windows utilities for process, memory, file system, and registry analysis.
Tripwire – File integrity monitoring tool used to detect system and file modifications.
lsof (List Open Files) – Utility for identifying files and resources currently accessed by running processes.
Wireshark – Network protocol analyzer used for capturing and analyzing network traffic.
Additional Monitoring Tools – Various utilities for process tracking, system auditing, log analysis, and behavioral monitoring.

<img width="740" height="480" alt="image" src="https://github.com/user-attachments/assets/81f21294-2b4f-40b2-a178-26eca09e1854" />


