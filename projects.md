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
### AI Surrogates for HPC Applications
#### Project (1) Constructing AI surrogate models for large-scale scientific applications 
This project focuses on designing and training AI-based surrogate models to approximate complex, large-scale scientific simulations. By capturing the essential dynamics of these simulations, the surrogate models can significantly speed up computation while maintaining high accuracy. 
-- Physics-informed machine learning
-- AutoML
-- Hybrid ML/numerical approaches 
Background reading: 
[1] SC’18: CosmoFlow: Using Deep Learning to Learn the Universe at Scale
[2] SC’19: Smart-PGSim: Using Neural Network to Accelerate AC-OPF Power Grid Simulation (Our paper)
[3] SC’20: Pushing the limit of molecular dynamics with ab initio accuracy to 100 million atoms with machine learning (Our paper)
[4] AlphaFold 1,2,3 
[5] SC’23: GenSLMs: Genome-scale language models reveal SARS-CoV-2 evolutionary dynamics
(Our works are pure AI surrogate works, others are AI for Science frameworks, i.e., replacing the whole applications with AI models)

#### Project (2) Adapting foundation AI models in HPC applications via understanding their dynamic program behaviors
In this project, we aim to adapt powerful, pre-trained foundation models (e.g., backbone models trained on a subject of datasets) to HPC applications. The key challenge is to analyze and understand the dynamic behavior of HPC programs so that we can fine-tune the foundation model to adapt to different downstream tasks (e.g., braches) effectively. 
A high-risk high-reward topic to explore. It is still in its early stages, but I have several HPC applications in my mind to explore! I love this project. Come and talk to me if you are interested. 

#### Project (3) Program-Insight Driven Code Selection for AI Surrogates
This project seeks to automatically identify the most beneficial parts of HPC applications that can be replaced or augmented by AI surrogates. By analyzing performance data and program characteristics, we will develop methodologies to select code segments where AI can offer the greatest speedup or efficiency gains. Students will engage in program analysis, surrogate model design, and algorithm/framework design for performance trade-offs.

Background reading: 
[1] HPDC’23: Auto-HPCnet: An Automatic Framework to Build Neural Network-based Surrogate for High-Performance Computing Applications (Our paper)
[2] SC’24: HPAC-ML: A Programming Model for Embedding ML Surrogates in Scientific Applications
[3] 2022: AI-coupled HPC Workflow Applications, Middleware and Performance
[4] 2024: AI-coupled HPC Workflows 
[5] 2024: Feasibility Study on Active Learning of Smart Surrogates for Scientific Simulations
[6] 2020: Using Machine Learning at scale in numerical simulations with SmartSim: An application to ocean climate modeling

One NSF project and one preliminary work (paper) are under submission.


### System optimization for Large-scale Scientific AI models
#### Project (1) Boosting the performance with cutting-edge AI accelerators (Cerebras, Sambanova, Groq, etc) 
This project investigates how emerging AI accelerator hardware can transform large-scale scientific AI workloads. Students will experiment with state-of-the-art processors—such as Cerebras, Sambanova, and Groq—to optimize model training and inference. The goal is to uncover new strategies for parallelism, memory management, and computation efficiency that push the limits of scientific AI performance.

Background reading:
[1] Steering Customized AI Architectures for HPC Scientific Applications
[2] Cerebras Architecture Deep Dive: First Look Inside the Hardware/Software Co-Design for Deep Learning

#### Project (2) Mitigating the memory bottleneck in scientific foundation AI models
Large-scale scientific models often face severe memory constraints when handling scientific data. In this project, we will develop techniques—such as model partitioning, sparsity, and on-the-fly compression—to alleviate memory bottlenecks in HPC and AI applications. Students will tackle system-level optimizations, explore hardware-aware methods, and build scalable solutions for next-generation scientific AI models.

-- Profiling the performance of scientific AI models such as throughputs, memory usage and data transfer or communication overhead, etc
-- System-level optimization such as kernel optimization, kernel optimization, load balance, and overlapping of communication and computation, etc  

Background reading: 
[1] Models: Awesome-Foundation-Models-for-Weather-and-Climate (https://github.com/shengchaochen82/Awesome-Foundation-Models-for-Weather-and-Climate)
[2] MLsys papers: FlashAttention, Zero, Zero-infinity, FlexLLMGen, FlashInfer, etc   



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

