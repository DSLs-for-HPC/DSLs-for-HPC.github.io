---
layout: page
# Index page
---

# CS8803-DSL: Domain Specific Languages for High Performance Computing
CRN-93621

This course will empower students to design and implement Domain-Specific programming Languages (DSLs) to solve problems in High-Performance Computing (HPC) contexts. Students will learn basics of compiler construction and language design as it relates to the challenges of high-performance computing and performance engineering. The course will cover topics such as architectural modelling, optimization techniques, and program analysis, through the context of contemorary DSLs and research in the field. It is my hope that any student taking the course will leave with the skills to build compilers to solve programming problems in their own HPC research areas. The course will be project-focused, with a few assignments and a final project to design and implement a DSL for some HPC problem.

## Learning Objectives

By the end of this course, students will be able to:
- Measure and analyze the performance of compilers and HPC programs.
- Design and implement languages to capture concepts in data/scientific domains.
- Embed/integrate DSLs in existing programming languages and frameworks.
- Adapt languages to model and target HPC architectures.
- Apply optimization techniques to improve the performance of generated programs. 
- Communicate technical concepts to build your career in academic contexts.

We will accomplish these objectives through a combination of homework problems, discussions, group peer review activities, and a special project.

## Policies

See the [Course Policies](policies) for more information on grading, assignments, and other course policies.

> **Note:** This course website is currently under construction. Please check back later for more information.

## Course Information

- **Course Code:** CS8803-DSL  
- **CRN:** 93621  
- **Credits:** 3  
- **Instructor:** Willow Ahrens ([willow@csail.mit.edu](mailto:willow@csail.mit.edu))  
- **Office Hours:** TBA
- **Meeting Room:** Arch 107  
- **Meeting Time:** Tuesday & Thursday, 12:30–1:45 PM

## Schedule

| Date | Topics | Readings | Notes |
|------|--------|----------|-------|
| August 19 | **Welcome**<br>• Why DSLs?<br>• Course Policies<br>• Course Overview | **Readings:**<br>• [Programming Pearls: Little Languages](https://doi.org/10.1145/6424.315691)<br>• [A New Golden Age for Computer Architecture](https://cacm.acm.org/research/a-new-golden-age-for-computer-architecture/)<br>• [How to Read a Paper](https://web.stanford.edu/class/cs245/readings/how-to-read-a-paper.pdf) | Slides (from Stanford CS343D) |
| August 21 | **Getting Started with DSLs**<br>• What is a DSL?<br>• Abstract Syntax Trees (ASTs)<br>• Lexical Analysis and Parsing<br>• Embedded DSLs (Lazy Evaluation, Functions, and Macros) | **Readings:**<br>• [Compilers: Principles, Techniques, and Tools, Chapter 4.1-4.3](https://dl.acm.org/doi/10.5555/1177220)<br>• [finch-tensor-lite embedded parser](https://github.com/finch-tensor/finch-tensor-lite/tree/main/src/finch/interface)<br>**Discussion:**<br>• [Terra: A Multi-Stage Language for High-Performance Computing](https://doi.org/10.1145/2491956.2462166) | Slides (from Stanford CS343D) |
| August 26 | **Measurement**<br>• What is Fast? Benchmarking and Performance Metrics<br>• Amdahl's Law<br>• Roofline Model<br>• Benchmarking Compilers | **Readings:**<br>• [Roofline: an insightful visual performance model for multicore architectures](https://dl.acm.org/doi/10.1145/1498765.1498785)<br>• [Scientific benchmarking of parallel computing systems: twelve ways to tell the masses when reporting performance results](https://doi.org/10.1145/2807591.2807644)<br>**Discussion:**<br>• [Producing wrong data without doing anything obviously wrong!](https://doi.org/10.1145/1508284.1508275)<br>• [PandasBench: A Benchmark for the Pandas API](https://arxiv.org/abs/2506.02345) | Slides (from UC Berkeley CS267) |
| August 28 | **Dense Array Programming / Loop Optimization**<br>• What is High-Performance Computing? An Overview<br>• Dense Array Programming<br>• Classical Optimizations: Loop Fusion, Loop Unrolling, Vectorization<br>• Mechanism Vs. Policy<br>• Halide | **Readings:**<br>• [Compilers: Principles, Techniques, and Tools, Chapter 10.4, 11.1, 11.2, 11.3, 11.7.8, 11.11](https://dl.acm.org/doi/10.5555/1177220)<br>**Discussion:**<br>• [Halide: decoupling algorithms from schedules for high-performance image processing](https://dl.acm.org/doi/10.1145/3150211)<br>• [Synthesis of High-Performance Parallel Programs for a Class of Ab Initio Quantum Chemistry Models](https://www.csc.lsu.edu/~gb/TCE/Publications/SynthApproach-ProcIEEE05.pdf) | Slides (from Stanford CS343D, Cornell CS 6120) |
| TBA | **Dataflow Analysis and Optimization**<br>• Program Analysis<br>• Dataflow Analysis<br>• Static vs. Dynamic Analysis<br>• Interval Analysis<br>• Heap Modeling | **Readings:**<br>• [Compilers: Principles, Techniques, and Tools, Second Edition, Chapter 9](https://dl.acm.org/doi/10.5555/1177220)<br>• [Lecture 4, Dataflow Analysis, Cornell CS 6120](https://www.cs.cornell.edu/courses/cs6120/2025sp/lesson/4/)<br>**Discussion:**<br>• [Representing Data Collections in an SSA Form](https://dl.acm.org/doi/10.1109/CGO57630.2024.10444817) | Slides (from Cornell CS 6120) |
| TBA | **Rewriting and Transformation**<br>• Rewriting Systems<br>• E-graphs | **Readings:**<br>• [Achieving high-performance the functional way: a functional pearl on expressing high-performance optimizations as rewrite strategies](https://steuwer.info/files/publications/2020/ICFP-Achieving-High-Performance-the-Functional-Way.pdf) ([CACM](https://dl.acm.org/doi/pdf/10.1145/3580371))<br>• [Software Design for Flexibility, Chapter 4](https://mitpress.mit.edu/9780262045490/software-design-for-flexibility/)<br>• [SymbolicUtils.jl](https://docs.sciml.ai/SymbolicUtils/stable/manual/rewrite/)<br>**Discussion:**<br>• [Spiral: Extreme Performance Portability via Generative Programming](https://doi.org/10.1109/JPROC.2018.2873289) | |
| TBA | **E-graphs**<br>• What is an E-graph?<br>• E-graph Representation<br>• Saturation, Search | **Readings:**<br>• [egg: Fast and extensible equality saturation](https://dl.acm.org/doi/10.1145/3434304)<br>**Discussion:**<br>• [Guided Equality Saturation](https://steuwer.info/files/publications/2024/POPL-Guided-Equality-Saturation.pdf)<br>• [Caviar: an e-graph based TRS for automatic code optimization](https://doi.org/10.1145/3497776.3517781) | Slides TBD |
| TBA | **Autotuning**<br>• What is Autotuning?<br>• Autotuning Frameworks<br>• Search Space Exploration | **Readings:**<br>• [Automatically tuned linear algebra software](https://dl.acm.org/doi/10.5555/509058.509096)<br>• [OpenTuner: An Extensible Framework for Program Autotuning](https://commit.csail.mit.edu/papers/2014/ansel-pact14-opentuner.pdf)<br>• [ATF: A Generic Auto-Tuning Framework](https://ieeexplore.ieee.org/document/8291912)<br>• [Autotuning in High-Performance Computing Applications](https://ieeexplore.ieee.org/document/8423171) | |
| TBA | **Sparse Array Programming**<br>• Domain: Sparse Arrays, Graphs, Meshes, Databases<br>• Representation (Sparse Matrix Formats, Columnar storage, Fibertree) | **Readings:**<br>• [Automatic Performance Tuning of Sparse Matrix Kernels](https://bebop.cs.berkeley.edu/pubs/vuduc2003-dissertation.pdf)<br>• [A relational model of data for large shared data banks](https://dl.acm.org/doi/10.1145/362384.362685)<br>**Discussion:**<br>• [The tensor algebra compiler](https://tensor-compiler.org/files/kjolstad-oopsla17-tensor-compiler.pdf)<br>• [Format abstraction for sparse tensor algebra compilers](https://doi.org/10.1145/3276493) | Slides (from Stanford CS343D) |
| TBA | **Sparse Array Programming Revisited**<br>• Coiteration (Merge Strategies, Looplets)<br>• Loops and Iteration<br>• Three Major Algorithms for Matrix Multiplication | **Readings:**<br>• [Gamma: Leveraging Gustavson's Algorithm to Accelerate Sparse Matrix Multiplication](https://dl.acm.org/doi/pdf/10.1145/3445814.3446702)<br>• [Looplets: A Language for Structured Coiteration](https://dl.acm.org/doi/10.1145/3579990.3580020)<br>• [Functional Collection Programming with Semi-ring Dictionaries](https://doi.org/10.1145/3527333) | |
| TBA | **Wild And Crazy Ideas Session**<br>• Bring a 5-min Slideshow on your crazy idea that just might work<br>• Peer Feedback <br>• Thinking about Final Projects | **Readings:**<br>•  | |
| TBA | **Vectorization**<br>• SSA Form<br>• Cleanup Strategies in Halide<br>• Auto-Vectorization | **Readings:**<br>• [All you need is superword-level parallelism: systematic control-flow vectorization with SLP](https://doi.org/10.5281/zenodo.6392272)<br>• [Vectorization in Halide](https://halide-lang.org/tutorials/tutorial_lesson_05_scheduling_1.html)<br>**Discussion:**<br>• [Vectorizing Sparse Matrix Computations with Partially-Strided Codelets](https://doi.org/10.1109/SC41404.2022.00037) | |
| TBA | **Multicore Parallelism**<br>• Multicore Architectures<br>• Parallel Programming Models<br>• Cilk | **Readings:**<br>• [The implementation of the Cilk-5 multithreaded language](https://dl.acm.org/doi/pdf/10.1145/277650.277725)<br>**Discussion:**<br>• [Heartbeat Scheduling: Provable Efficiency for Nested Parallelism](https://www.chargueraud.org/research/2018/heartbeat/heartbeat.pdf)<br>• [Tapir: Embedding Fork-Join Parallelism into LLVM's Intermediate Representation](https://dl.acm.org/doi/pdf/10.1145/3018743.3018758) | Slides (from UC Berkeley CS267, MIT 6.172) |
| TBA | **Distributed Memory Parallelism**<br>• Distributed Memory Architectures<br>• Message Passing Interface (MPI)<br>• MapReduce<br>• UPC<br>• Legion<br>• Communication-avoiding Matrix Multiply | **Readings:**<br>• [MapReduce: Simplified Data Processing on Large Clusters](https://doi.org/10.1145/1327452.1327492)<br>• [DISTAL: The Distributed Tensor Algebra Compiler](https://doi.org/10.1145/3519939.3523437)<br>• [Legion: Expressing Locality and Independence with Logical Regions](https://legion.stanford.edu/pdfs/sc2012.pdf)<br>• [Cyclops Tensor Framework](https://ieeexplore.ieee.org/document/6569864) | Slides (from UC Berkeley CS267) |
| TBA | **Accelerators and GPUs**<br>• GPU Programming Languages<br>• Data Parallel Languages | **Discussion:**<br>• [Taichi: a language for high-performance computation on spatially sparse data structures](https://doi.org/10.1145/3355089.3356506)<br>• [Task-Based Tensor Computations on Modern GPUs](https://d1qx31qr3h6wln.cloudfront.net/publications/Cypress_PLDI_25.pdf) | Slides (from UC Berkeley CS267) |
| TBA | **Staged Programming**<br>• What is Staged Programming?<br>• Abstract Interpretation<br>• Implementations | **Readings:**<br>• [Lightweight modular staging: a pragmatic approach to runtime code generation and compiled DSLs](https://doi.org/10.1145/1868294.1868314)<br>**Discussion:**<br>• [BuildIt: A Type-Based Multi-stage Programming Framework for Code Generation in C++](https://doi.org/10.1109/CGO51591.2021.9370333) | |
| TBA | **Dense Array Programming Revisited**<br>• Revisiting Dense Array Programming | **Readings:**<br>• [A Practical Automatic Polyhedral Parallelizer and Locality Optimizer](https://doi.org/10.1145/1375581.1375595)<br>• [The Pochoir Stencil Compiler](https://doi.org/10.1145/1989493.1989508)<br>**Discussion:**<br>• [Exocompilation for Productive Programming of Hardware Accelerators](https://dl.acm.org/doi/pdf/10.1145/3519939.3523446) | |
| TBA | **Autoscheduling**<br>• What is Autoscheduling?<br>• Three Ingredients of Autoscheduling (Search Space, Search Strategy, Cost Model)<br>• Autotuning vs. Autoscheduling<br>• Search Space Characterization<br>• Search Strategies | **Readings:**<br>• [Learning to Optimize Halide with Tree Search and Random Program](https://halide-lang.org/papers/autoscheduler2019.html) | TBD slides |
| TBA | **Autoscheduling Revisited**<br>• Cost Modeling (Feature-based/ML, Sparse Cost Models/Cardinality Estimation) | **Readings:**<br>• [How to Architect a Query Compiler](https://doi.org/10.1145/2882903.2915244)<br>• [Autoscheduling for sparse tensor algebra with an asymptotic cost model](https://doi.org/10.1145/3519939.3523442)<br>**Discussion:**<br>• [Galley: Modern Query Optimization for Sparse Tensor Programs](https://doi.org/10.1145/3519939.3523440) | TBD slides |
| TBA | **Compiling Programs Faster**<br>• Compilation Time vs. Execution Time<br>• Prepared queries<br>• Intepreters vs. Compilers<br>• Turn off Compilation | **Readings:**<br>• [Firefox's Baseline WebAssembly Compiler](https://hacks.mozilla.org/2018/01/making-webassembly-even-faster-firefoxs-new-streaming-and-tiering-compiler/)<br>**Discussion:**<br>• [Copy-and-Patch Compilation](https://fredrikbk.com/copy-and-patch.html) | Slides (from Stanford CS343D) |
| TBA | **Final Project Session**<br>• Bring a 5-min Slideshow on your crazy idea that just might work<br>• Peer Feedback <br>• Thinking about Final Projects | **Readings:**<br>•  | |

## Inspired by
- [Stanford CS343D: Domain-Specific Programming Models and Compilers](https://cs343d.github.io/course_info.html), Fredrik Kjolstad.
- [MIT 6.172: Performance Engineering of Software Systems](https://ocw.mit.edu/courses/6-172-performance-engineering-of-software-systems-fall-2018/),
- [Cornell CS 6120: Advanced Compilers](https://www.cs.cornell.edu/courses/cs6120/2025sp/syllabus/)
- [UC Berkeley CS267: Applications of Parallel Computers](https://sites.google.com/lbl.gov/cs267-spr2022), Aydin Buluc, Kathy Yelick, James Demmel.
- [UC Berkeley CS294: Building User-Centered Programming Tools](https://schasins.com/cs294-usable-programming-2025/)