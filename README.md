# QEC21 Workshop: Progress and Challenges in Quantum Intermediate Representations

The 2021 quantum intermediate representations workshop is hosted at IEEE Quantum Week, the IEEE International Conference on Quantum Computing and Engineering (QCE).

[Conference and workshop registration](https://qce.quantum.ieee.org/registration/registration-overview/)

The virtual workshop will be held online on Friday, Oct 22 10:45-16:45 Mountain Time (MDT) — UTC-6.

## Description

The goal of this workshop is to provide a platform for discussing current state-of-the-art approaches to quantum intermediate representation development, expression, deployment, and utility.
We will highlight recent approaches, future directions, and novel designs through a series of invited presentations and panel discussions on specific challenge topics from leaders in the field of quantum compilation.

*The abstract of the workshop can also be found on IEEE Quantum Week's [website](https://qce.quantum.ieee.org/workshops-program/#alexandermccaskey)*.

## Invited Speakers and Moderators

- Ken Brown (Duke)
- Thomas Alexander (IBM)
- Itamar Sivan (Quantum Machines)
- Ross Duncan (CQC)
- Wim Lavrijsen (LBL)
- Will Zeng (Unitary Fund)
- Blake Johnson (IBM)
- Eric Holland (Keysight)
- Steven Heidel (Amazon)
- Andrew Landahl (Sandia)
- Alex Chernoguzov (Honeywell)
- Bettina Heim (Microsoft)
- Thomas Haner (Microsoft)
- Kesha Hietala (University of Maryland)
- Benjamin Bichsel (ETH-Zurich)
- Alan Geller (Microsoft)
- Yunong Shi (Amazon)

## Program

### Session 1:  Interacting with Physical Hardware
#### 10:45-12:15 Mountain Time

_Exactly how much knowledge of the electronic control system does the IR need to possess? Do we need explicit wall clock timing? Should IRs have knowledge of analog pulse control?_
 
**Moderator: Ken Brown (Duke)**
- Presentations (20 min each) 
  - Thomas Alexander (IBM)
  - Itamar Sivan (Quantum Machines)
- Panel Discussion (50 min)
  - Ross Duncan (CQC)
  - Wim Lavrijsen (LBL)
  - Prakash Murali (Microsoft)

### Break: 12:15 PM - 12:45 PM 

### Session 2: Classical Control and Feedback
#### 12:45-14:15 PM Mountian Time

_Focus on the interplay between an IR and the classical infrastructure involved in fast-feedback and classical control. How does one handle and manage latency for measurement-based control flow?_

**Moderator: Will Zeng (Unitary Fund)**

- Presentations (20 min each) 
  - Blake Johnson (IBM)
  - Eric Holland (Keysight)
- Panel Discussion (50 min)
  - Steven Heidel (Amazon)
  - Andrew Landahl (Sandia)
  - Alex Chernoguzov (Honeywell)

### Break: 14:15 PM - 14:45 PM

### Session 3: Program Analysis and Memory Management
#### 14:45-16:15 PM Mountian Time

_At some point, QPUs will go beyond a single global register with some predefined connectivity. For example, we will need floating and fixed point arithmetic, or we might have specialized areas of processors dedicated to specific tasks like T-state generation. How should the IR relate to this?_

**Moderator: Bettina Heim (Microsoft)**

- Presentations (20 min each) 
  - Thomas Haner (Microsoft)
  - Kesha Hietala (University of Maryland)
- Panel Discussion (50 min)
  - Benjamin Bichsel (ETH-Zurich)
  - Alan Geller (Microsoft)
  - Yunong Shi (Amazon)

### Extra discussion time: 16:15 PM - 16:45 P

_You can find a full or compact view of the complete [QCE21 Program](https://qce.quantum.ieee.org/workshops-program/) on their website._

## Talk Abstracts

### Co-designing programming representations, runtimes, and control systems for layered control of quantum hardware
#### Thomas Alexander (IBM)

Current quantum computers consist of systems of heterogeneous equipment that we orchestrate to execute an input quantum program. Using a layered system of abstractions consisting of program binaries, a hardware abstraction layer, pulse, and quantum circuits we obtain a scalable framework for compiling and executing quantum programs across a configurable spectrum of quantum systems. In our talk, we will introduce the components of this framework and the lessons we have learned from deploying, maintaining, programming, and supporting quantum hardware for extended periods.

### Challenges in the emerging IR ecosystem
#### Itamar Sivan (Quantum Machines)

Intermediate representations (IRs) are an essential element for a thriving ecosystem of programmers, programming languages and programming tools. The IR role is primarily to ease the introduction and compatibility of languages, compilers and processors. In a mature stack, this allows the formation of a healthy ecosystem in which migration across tools and languages is done with ease. However, IRs in an emerging stack may also pose a challenge since, if not defined well, the IR can add challenging constraints or conceal advanced capabilities from arriving at users' disposal. In this talk we will discuss these challenges in the emerging quantum computing ecosystem and propose exciting ways to face them.

### Synchronous execution in distributed control systems
#### Blake Johnson (IBM)

There are two predominant models of control system architectures found in the wild: centralized and distributed. We will take a brief look at each to discover why the distributed model is more common. While having distinct benefits, the distributed model also carries certain challenges in maintaining synchronous execution on such systems. We will look at a couple example circuits to discover some desired properties in systems built to define the microcode that implements quantum operations on such controllers.

### Quantum Intermediate Representations and Classical Control Flow
#### Eric Holland (Keysight)
Quantum computing continues to make great strides towards the ultimate goal of universal fault tolerant quantum computation. 
However, as the field matures and expands there are open questions on how to leverage lessons learned from more than 80 years of classical computing success.
In this talk I will present the challenges, opportunities, and questions facing the field over the coming years at the intersection of quantum intermediate representations (QIR) and classical control flow.
For instance, as specialization continues to emerge, how do we maintain abstraction for reuse and intercompatibility for deployed quantum cloud systems as well as enable maintain flexibility and expressiveness for the underlying R&D at all levels of the quantum computing stack?
The answer to these questions will heavily influence what and how is represented in a QIR as well as the interface to classical control flow.

### Quantum IRs for optimization and resource estimation
#### Thomas Haner (Microsoft)
With an increasing number of quantum devices accessible through the cloud, several new representations for hybrid quantum-classical programs have recently been proposed.
Furthermore, there have been recent advances on the classical side such as MLIR, which was introduced to facilitate implementing language- and domain-specific IRs.
In this talk, I will highlight challenges in compiling quantum programs that may be tackled with such frameworks.
Specifically, I will be focusing on optimization and resource estimation of quantum programs.

### Quantum Intermediate Representations for Formal Verification
#### Kesha Hietala (University of Maryland)

Formal verification is the process of mathematically proving that a design matches a specification. It can be used to provide guarantees about the behavior of software on all possible inputs, making it especially powerful in domains like quantum programming, where intermediate state collapse and hardware errors complicate standard software assurance techniques. At the University of Maryland, we have been working on formally verifying quantum algorithms and circuit optimizations. To facilitate this work, we designed an intermediate representation, SQIR, and gave it a formal semantics in the Coq proof assistant. We have verified the correctness of key quantum algorithms implemented in SQIR and state-of-the-art optimizations over SQIR programs. In this talk, I will present our prior and ongoing work on designing quantum intermediate representations suitable for formal verification.

## Organizers

- Alexander McCaskey: Oak Ridge National Laboratory (ORNL), USA
- Bettina Heim: Microsoft, USA
- Yudong Cao: Zapata Computing, USA
- Will Zeng: Unitary Fund, USA
- Sarah Kaiser: Unitary Fund, USA
