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

Assembly is the lowest level in the software chain and although we don’t have access to the source code, various tools can reduce the source code to assembly. Each instruction in any higher level language must be visible to the assembly language code. There is no magic here, each instruction must be reduced to one or more assembly instructions. In most cases, we will be working with this simple assembly code when reverse engineering.

Obviously, to be successful at reversing, we must be familiar with assembly language code. Unfortunately, there is not a single assembly language, but rather an assembly language for each type of processor (x86, x64, ARM, PPC, etc). To master reversing, we must master the assembly code of our chosen platform. In this series, we will be examining x86, x64 and ARM assembly.

<img width="740" height="399" alt="image" src="https://github.com/user-attachments/assets/6c5a0d3e-c3dc-4ce7-a1fb-ce8f7262a4f0" />

When we do code level reversing, we are attempting to extract the software’s code concepts and algorithms from the machine code. This requires a solid understanding of such things as how the CPU works, how the operating system works and the process of software development. We will be using such tools as IDA Pro, SoftIce, Ollydbg, Ghidra and some others in this process.

<img width="740" height="435" alt="image" src="https://github.com/user-attachments/assets/3e84a8da-0318-4ced-b47f-0430489541f2" />

System level reversing involves running tools to obtain information about the software, inspect the program, inspect the executables, and track the program’s input and output. Most of this information will come from the operating system. We will be using such tools as SysInternals Suite, Tripwire, lsof, Wireshark, and others.

<img width="740" height="480" alt="image" src="https://github.com/user-attachments/assets/81f21294-2b4f-40b2-a178-26eca09e1854" />


