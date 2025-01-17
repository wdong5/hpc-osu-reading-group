# Collaborative Projects

Here are project ideas from the PIs. 

## Renato

## Kyle

### Virtines 
This project involves developing a software framework
for lightweight, bespoke, virtualized execution contexts that we call Colony. Colony leverages
novel execution abstractions tailored to the application and designed
for both performance and isolation _from the ground up_. Colony contexts
are synthesized based on novel compiler analyses, and are exposed through
a rich set of programming abstractions and language extensions. Colony builds
on a new abstraction for isolated function execution, the
virtualized subroutine, or _virtine_, along with a prototype embeddable
hypervisor called Wasp. The goal of the Colony project is to achieve both high
performance and strong isolation for individually isolated function contexts in
a variety of applications.
The project will explore various mechanisms to enable bespoke
contexts, including virtualization mechanisms enhanced for optimized start-up
performance, and programming models with language/compiler support. The
security and isolation properties of bespoke contexts will also be explored.

**Background Reading**: Our [EuroSys '22 paper](https://dl.acm.org/doi/10.1145/3492321.3519553).

This project is funded by my CAREER grant. 

### Coalescent Computing

This project sits at the intersection of edge computing, distributed systems, and OS/virtualization. The basic
idea is to allow edge/mobile devices to _transparently_ borrow resources from one another. Think about a scenario
where you walk into a coffee shop, and your laptop automatically attaches to the CPU cores, memory, GPUs, accelerators, etc.
of other users' systems. Imagine running htop to see new CPU cores appear (and disappear) as you walk around the building. 
This (very early stage) project would involve exploring this idea. 

**Background Reading**: My [vison paper](https://dl.acm.org/doi/10.1145/3476886.3477503) at APSys '21. 

### PIM

This project focuses on memory-centric computing. In particular, we target novel processing-in-memory (PIM) devices. 
Current software support for such devices, e.g., [UPMEM](https://www.upmem.com/) is very limited. Our part of this work
would invovle:
- Evolving the OS kernel’s device driver interface for PIM, and
- Enhancing OS resource management capabilities for PIM

This is a collaborative NSF-funded project with Xian-He Sun @ IIT and Peng Jiang @ The University of Iowa, and would
likely involve working with students from those institutions. 

No publications to date on this project, but you can an overview of PIM [here](https://arxiv.org/abs/2012.03112). 

### CARDS

This project involves improving compiler support for disaggregated memory (in particular, far memory). 
The basic idea is that kernel-based far memory swap introduces performance overheads (I/O amplification), 
and library-based approaches to far memory introduce programmer burden. The compiler approach strikes
a middle ground by transforming a legacy application to use far memory. 

Our initial work demonstrates the utility of the idea. The current effort, compiler-assisted remote datastructures (CARDS)
involves extending our TrackFM compiler to explore novel prefetching techniques, better support for recursive data structures, and coming up with better policies for remoting. 

**Background Reading**: Our [ASPLOS '24 paper](https://dl.acm.org/doi/10.1145/3617232.3624856)

I will be submitting a grant to support this work soon. 

## Wenqian


# Project Interest

Please indicate your interest here by putting down your name under projects you'd consider contributing to. This doesn't
mean you need to lead the project, it might just mean you want to sit in on related meetings, or brainstorm potential overlap
of that project with your current work. 

- [Virtines](#virtines)
  * Kyle
- [Coalescent Computing](#coalescent-computing)
  * Kyle
- [PIM](#pim)
  * Kyle
- [CARDS](#cards)
  * Kyle

