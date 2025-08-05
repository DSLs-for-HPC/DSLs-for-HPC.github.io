---
layout: page
# Index page
---

# CS8803-DSL: Domain Specific Languages for High Performance Computing
CRN-93621

This course will empower students to design and implement domain-specific programming languages (DSLs) to solve problems in high-performance computing (HPC) contexts. Students will learn basics of compiler construction and language design as it relates to the challenges of high-performance computing and performance engineering. The course will cover topics such as architectural modelling, optimization techniques, and program analysis, through the context of contemorary DSLs and research in the field. The course will be project-focused, with a few assignments and a final project to design and implement a DSL for some HPC problem.

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

### Intro
- Topics:
    - Why DSLs?
    - Course Policies
    - Course Overview
- Readings:
    - [Programming Pearls: Little Languages](https://dl.acm.org/doi/10.1145/6424.315691)
    - [A New Golden Age for Computer Architecture](https://cacm.acm.org/research/a-new-golden-age-for-computer-architecture/)
    - [How to Read a Paper](https://web.stanford.edu/class/cs245/readings/how-to-read-a-paper.pdf)
- Slides:
    - Stanford CS343D

### Getting Started with DSLs
- Topics:
    - What is a DSL?
    - Abstract Syntax Trees (ASTs)
    - Lexical Analysis and Parsing
    - Embedded DSLs (Lazy Evaluation, Functions, and Macros)
- Readings::
    - [Compilers: Principles, Techniques, and Tools, by Alfred V. Aho, Monica S. Lam, Ravi Sethi, and Jeffrey D. Ullman, Second Edition, Chapter 4.1-4.3](TODO)
    - [Functional Programming for Domain-Specific Languages](https://www.cs.ox.ac.uk/jeremy.gibbons/publications/fp4dsls.pdf)
    - [finch-tensor-lite embedded parser](https://github.com/finch-tensor/finch-tensor-lite/tree/main/src/finch/interface)
- Discussion:
    - [Terra: A Multi-Stage Language for
High-Performance Computing](doi.org/10.1145/2491956.2462166)
- Slides:
    - Stanford CS343D

### Measurement
- Topics:
    - What is Fast? Benchmarking and Performance Metrics
    - Amdahl's Law
    - Roofline Model
    - Benchmarking Compilers
- Readings:
    - [Roofline: an insightful visual performance model for multicore architectures](https://dl.acm.org/doi/10.1145/1498765.1498785)
    - [Scientific benchmarking of parallel computing systems: twelve ways to tell the masses when reporting performance results](https://doi.org/10.1145/2807591.2807644)
- Discussion:
    - [Producing wrong data without doing anything obviously wrong!](https://doi.org/10.1145/1508284.1508275)
    - [PandasBench: A Benchmark for the Pandas API](https://arxiv.org/abs/2506.02345)
- Slides:
    - UC Berkeley CS267

### Dense Array Programming / Loop Optimization
- Topics:
    - What is High-Performance Computing? An Overview
    - Dense Array Programming
    - Classical Optimizations: Loop Fusion, Loop Unrolling, Vectorization
    - Mechanism Vs. Policy
    - Halide
- Readings:
    - [Compilers: Principles, Techniques, and Tools, by Alfred V. Aho, Monica S. Lam, Ravi Sethi, and Jeffrey D. Ullman, Second Edition, Chapter 10.4, 11.1, 11.2, 11.3, 11.7.8, 11.11](TODO)
- Discussion:
    - [Halide: decoupling algorithms from schedules for high-performance image processing](https://dl.acm.org/doi/10.1145/3150211)
    - [Synthesis of High-Performance Parallel Programs for a Class of Ab Initio Quantum Chemistry Models](https://www.csc.lsu.edu/~gb/TCE/Publications/SynthApproach-ProcIEEE05.pdf)
- Slides:
    - Stanford CS343D
    - Cornell CS 6120

### Dataflow Analysis and Optimization
- Topics:
    - Program Analysis
    - Dataflow Analysis
    - Static vs. Dynamic Analysis
    - Interval Analysis
    - Heap Modeling
- Readings:
    - [Compilers: Principles, Techniques, and Tools, by Alfred V. Aho, Monica S. Lam, Ravi Sethi, and Jeffrey D. Ullman, Second Edition, Chapter 9](TODO)
    - [Lecture 4, Dataflow Analysis, Cornell CS 6120](https://www.cs.cornell.edu/courses/cs6120/2025sp/lesson/4/)
- Discussion:
    - [Representing Data Collections in an SSA Form](https://dl.acm.org/doi/10.1109/CGO57630.2024.10444817)
- Slides:
    - Cornell CS 6120

### Rewriting and Transformation
- Topics:
    - Rewriting Systems
    - E-graphs
- Readings:
    - [Achieving high-performance the functional way: a functional pearl on expressing high-performance optimizations as rewrite strategies](https://steuwer.info/files/publications/2020/ICFP-Achieving-High-Performance-the-Functional-Way.pdf) [CACM](https://dl.acm.org/doi/pdf/10.1145/3580371)
    - [Software Design for Flexibility, Chapter 4](https://mitpress.mit.edu/9780262045490/software-design-for-flexibility/)
    - [SymbolicUtils.jl](https://docs.sciml.ai/SymbolicUtils/stable/manual/rewrite/)
- Discussion:
    - [Spiral: Extreme Performance Portability via Generative Programming](https://doi.org/10.1109/JPROC.2018.2873289)

### E-graphs
- Topics:
    - What is an E-graph?
    - E-graph Representation
    - Saturation, Search
- Readings:
    - [egg: Fast and extensible equality saturation](https://dl.acm.org/doi/10.1145/3434304)
- Discussion:
    - [Guided Equality Saturation](https://steuwer.info/files/publications/2024/POPL-Guided-Equality-Saturation.pdf)
    - [Caviar: an e-graph based TRS for automatic code optimization](https://doi.org/10.1145/3497776.3517781)
- Slides:
    - TBD

### Autotuning
- Topics:
    - What is Autotuning?
    - Autotuning Frameworks
    - Search Space Exploration
- Readings:
    - [Automatically tuned linear algebra software](https://dl.acm.org/doi/10.5555/509058.509096)
    - [OpenTuner: An Extensible Framework for Program Autotuning](https://commit.csail.mit.edu/papers/2014/ansel-pact14-opentuner.pdf)
    - [ATF: A Generic Auto-Tuning Framework](https://ieeexplore.ieee.org/document/8291912)
    - [Autotuning in High-Performance Computing Applications](https://ieeexplore.ieee.org/document/8423171)

### Sparse Array Programming
- Topics:
    - Domain: Sparse Arrays, Graphs, Meshes, Databases
    - Representation
        - Sparse Matrix Formats
        - Columnar storage
        - Fibertree
- Readings: 
    - [Automatic Performance Tuning of Sparse Matrix Kernels](https://bebop.cs.berkeley.edu/pubs/vuduc2003-dissertation.pdf)
    - [A relational model of data for large shared data banks](https://dl.acm.org/doi/10.1145/362384.362685)
- Discussion:
    - [The tensor algebra compiler](http://tensor-compiler.org/files/kjolstad-oopsla17-tensor-compiler.pdf)
    - [Format abstraction for sparse tensor algebra compilers](https://doi.org/10.1145/3276493)
- Slides:
    - Stanford CS343D
    
### Sparse Array Programming Revisited
- Topics:
    - Coiteration
        - Merge Strategies
        - Looplets
    - Loops and Iteration
        - Three Major Algorithms for Matrix Multiplication
- Readings:
    - [Gamma: Leveraging Gustavson’s Algorithm to Accelerate Sparse Matrix Multiplication](https://dl.acm.org/doi/pdf/10.1145/3445814.3446702)
    - [Looplets: A Language for Structured Coiteration](https://dl.acm.org/doi/10.1145/3579990.3580020)
    - [Functional Collection Programming with Semi-ring Dictionaries](https://doi.org/10.1145/3527333)
- Slides:
    - TODO

### Vectorization
- Topics:
    - SSA Form
    - Cleanup Strategies in Halide
    - Auto-Vectorization
- Readings:
    - [All you need is superword-level parallelism: systematic control-flow vectorization with SLP](https://doi.org/10.5281/zenodo.6392272)
    - [Vectorization in Halide](https://halide-lang.org/tutorials/tutorial_lesson_05_scheduling_1.html)
- Discussion:
    - [Vectorizing Sparse Matrix Computations with Partially-Strided Codelets](doi.org/10.1109/SC41404.2022.00037)
- Slides:

### Multicore Parallelism
- Topics:
    - Multicore Architectures
    - Parallel Programming Models
    - Cilk
- Readings:
    - [https://dl.acm.org/doi/pdf/10.1145/277650.277725](https://dl.acm.org/doi/10.1145/277650.277725)
- Discussion:
    - [Heartbeat Scheduling: Provable Efficiency for Nested Parallelism](https://www.chargueraud.org/research/2018/heartbeat/heartbeat.pdf)
    - [Tapir: Embedding Fork-Join Parallelism into LLVM’s Intermediate Representation](https://dl.acm.org/doi/pdf/10.1145/3018743.3018758)
- Slides:
    - UC Berkeley CS267
    - MIT 6.172

### Distributed Memory Parallelism
- Topics:
    - Distributed Memory Architectures
    - Message Passing Interface (MPI)
    - MapReduce
    - UPC
    - Legion
    - Communication-avoiding Matrix Multiply
- Readings:
    - [MapReduce: Simplified Data Processing on Large Clusters](https://storage.googleapis.com/gweb-research2023-media/pubtools/4449.pdf)
    - [DISTAL: The Distributed Tensor Algebra Compiler](https://dl.acm.org/doi/pdf/10.1145/3519939.3523437)
    - [Legion: Expressing Locality and Independence with Logical Regions](https://legion.stanford.edu/pdfs/sc2012.pdf)
    - [Cyclops Tensor Framework: Reducing Communication and Eliminating Load Imbalance in Massively Parallel Contractions](https://ieeexplore.ieee.org/document/6569864)
- Slides:
    - UC Berkeley CS267

### Accelerators and GPUs
- Topics:
    - GPU Programming Languages
    - Data Parallel Languages
- Readings:
- Discussion:
    - [Taichi: a language for high-performance computation on spatially sparse data structures](https://doi.org/10.1145/3355089.3356506)
    - [Task-Based Tensor Computations on Modern GPUs](https://d1qx31qr3h6wln.cloudfront.net/publications/Cypress_PLDI_25.pdf)
    - 
- Slides:
    - UC Berkeley CS267

### Staged Programming
- Topics:
    - What is Staged Programming?
    - Abstract Interpretation
    - Implementations
- Readings:
    - [Lightweight modular staging: a pragmatic approach to runtime code generation and compiled DSLs](https://doi.org/10.1145/1868294.1868314)
- Discussion:
    - [BuildIt: A Type-Based Multi-stage Programming Framework for Code Generation in C++](https://doi.org/10.1109/CGO51591.2021.9370333)


### Dense Array Programming Revisited
- Topics:
    - Revisiting Dense Array Programming
- Readings:
    - [A Practical Automatic Polyhedral Parallelizer and Locality Optimizer](https://doi.org/10.1145/1375581.1375595)
    - [The Pochoir Stencil Compiler](https://doi.org/10.1145/1989493.1989508)
- Discussion:
    - [Exocompilation for Productive Programming of Hardware Accelerators](https://dl.acm.org/doi/pdf/10.1145/3519939.3523446)

### Autoscheduling
- Topics:
    - What is Autoscheduling?
    - Three Ingredients of Autoscheduling
        - Search Space
        - Search Strategy
        - Cost Model
    - Autotuning vs. Autoscheduling
    - Search Space Characterization
    - Search Strategies
- Readings:
    - [Learning to Optimize Halide with Tree Search and Random Program](https://halide-lang.org/papers/autoscheduler2019.html)
    -
- Slides:
    TBD
    
### Autoscheduling Revisited
- Topics:
    - Cost Modeling
        - Feature-based/ML
        - Sparse Cost Models/Cardinality Estimation
- Readings:
    - [How to Architect a Query Compiler](https://doi.org/10.1145/2882903.2915244)
    - [Autoscheduling for sparse tensor algebra with an asymptotic cost model](https://doi.org/10.1145/3519939.3523442)
- Discussion:
    - [Galley: Modern Query Optimization for Sparse Tensor Programs](https://doi.org/10.1145/3519939.3523440)
- Slides:
    - TBD

### Compiling Programs Faster
- Topics:
    - Compilation Time vs. Execution Time
    - Prepared queries
    - Intepreters vs. Compilers
    - Turn off Compilation
- Readings:
    - [Firefox's Baseline WebAssembly Compiler](https://hacks.mozilla.org/2018/01/making-webassembly-even-faster-firefoxs-new-streaming-and-tiering-compiler/)
- Discussion:
    - [Copy-and-Patch Compilation](https://fredrikbk.com/copy-and-patch.html)
- Slides:
    - Stanford CS343D

## Inspired by
- [Stanford CS343D: Domain-Specific Programming Models and Compilers](https://cs343d.github.io/course_info.html), Fredrik Kjolstad.
- [MIT 6.172: Performance Engineering of Software Systems](https://ocw.mit.edu/courses/6-172-performance-engineering-of-software-systems-fall-2018/),
- [Cornell CS 6120: Advanced Compilers](https://www.cs.cornell.edu/courses/cs6120/2025sp/syllabus/)
- [UC Berkeley CS267: Applications of Parallel Computers](https://sites.google.com/lbl.gov/cs267-spr2022), Aydin Buluc, Kathy Yelick, James Demmel.
- [UC Berkeley CS294: Building User-Centered Programming Tools](https://schasins.com/cs294-usable-programming-2025/)