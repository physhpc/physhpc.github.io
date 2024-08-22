---
layout: default
---

# Program and Abstracts

<!-- TBA -->

**Date: August 27, 202 - Room: -1.A.02**

Chair: Francesco Pucci

- 13:30 - 14:10  - **Fabio Bacchini - Keynote talk**\\
> 
\\
**Title**. Computational astroplasma simulations: state of the art and future directions\\
\\
**Abstract**. Massively parallel computer codes are the paramount standard for simulations of astrophysical plasmas in modern scientific research. From the solar environment to the surroundings of supermassive black holes, simulations have helped shed light on many previously unknown processes concerning plasmas in the Universe. Given the very limited space offered by analytic calculations, continuing efforts devoted to the development of modern, reliable simulations tools are imperative. In this talk, I will review the main computing approaches employed in modern astroplasma research, and focus on the challenges and opportunities offered by the newest computing technologies on the market. 


- 14:10 - 14:30 - M. Battarbee, K. Papadakis, U. Ganse, J. Hokkanen, Y. Pfau-Kempf, M. Alho, and M. Palmroth.
>
\\
**Title**. Vlasiator: a global magnetospheric ion-kinetic plasma simulation in the age of GPU supercomputing\\
\\
**Abstract**. Vlasiator is a space plasma simulation code which models near-Earth collisionless ion-kinetic plasma dynamics in three spatial and three velocity dimensions. It is highly parallelized, modeling the Vlasov equation directly through the distribution function, discretized on a Cartesian grid, instead of the more common particle-in-cell approach. Vlasiator solves the Vlasov equation in the ion-kinetic hybrid formalism, modelling ions directly through the distribution function, with electrons included as a charge-neutralizing fluid. Modeling near-Earth space, plasma properties span several orders of magnitude in temperature, density, and magnetic field. We introduce some recent Vlasiator highlights, as well as talk about future plans.
In order to fit the required six-dimensional grids in memory, Vlasiator utilizes a sparse block-based velocity mesh, where chunks of velocity space are added or deleted based on the advection requirements of the Vlasov solver. In addition, the spatial mesh is adaptively refined through cell-based octree refinement. With these innovations, global 6D simulations have been achieved with the fastest CPU-based supercomputers in the world. With the advent of exascale, Vlasiator is being extended to support heterogeneous CPU/GPU architectures. We discuss memory management, algorithmic changes, and kernel construction as well as our unified codebase approach, resulting in portability to both NVIDIA and AMD hardware (CUDA and HIP languages, respectively). We present current performance metrics, discuss some newly developed parallel agorithms, and lay out a plan for optimization to facilitate future exascale simulations using multi-node GPU supercomputing.

- 14:30 - 14:50 - K. Schoeffler
> 
\\
**Title**. Numerical techniques for new advanced high-energy-density laser plasmas\\
\\
**Abstract**. In modern times, plasma effects have been modeled using massively parallel simulation techniques to further understanding of space and astrophysical phenomena as well as the results of laboratory experiments. Recent advances open the possibility for laser experiments to produce plasmas in extreme regimes, comparable to some astrophysical environments, where effects such as radiation reaction and even antimatter-pair production become important. In order to properly study these regimes which continue to be computationally challenging, new numerical algorithms for the exotic physics involved must be developed. In this talk, I will review state-of-the-art numerical techniques used to model these unique high-energy environments.

- 14:50 - 15:10 - J. Williams, S. Costea, A. Malony, D. Tskhakaya, L. Kos, A. Podolnik, J. Hromadka, K. Huck, E. Laure, and S. Markidis.\\
> 
\\
**Title**. Understanding the Impact of openPMD on BIT1, a Particle-in-Cell Monte Carlo Code, through Instrumentation, Monitoring, and In-Situ Analysis\\
\\
**Abstract**. Particle-in-Cell Monte Carlo simulations on large-scale systems play a fundamental role in understanding the complexities of plasma dynamics in fusion devices. Efficient handling and analysis of vast datasets are essential for advancing these simulations. Previously, we addressed this challenge by integrating openPMD with BIT1, a Particle-in-Cell Monte Carlo code, streamlining data streaming and storage. This integration not only enhanced data management but also improved write throughput and storage efficiency. In this work, we delve deeper into the impact of BIT1 openPMD BP4 instrumentation, monitoring, and in-situ analysis. Utilizing cutting-edge profiling and monitoring tools such as gprof, CrayPat, Cray Apprentice2, IPM, and Darshan, we dissect BIT1's performance post-integration, shedding light on computation, communication, and I/O operations. Fine-grained instrumentation offers insights into BIT1's runtime behavior, while immediate monitoring aids in understanding system dynamics and resource utilization patterns, facilitating proactive performance optimization. Advanced visualization techniques further enrich our understanding, enabling the optimization of BIT1 simulation workflows aimed at controlling plasma-material interfaces with improved data analysis and visualization at every checkpoint without causing any interruption to the simulation.

- 15:10 - 15:30 Coffee break

Chairs: Nicola Gullo, Donato D'Ambrosio 

- 15:30 - 16:10 - **Andrea Marini - Keynote talk**: 
> 
\\
**Title**. Simulations of out–of–equilibrium phenomena using the Yambo project\\
\\
**Abstract**. FLASH (Free Electron Laser in Hamburg) and Lumi (Large Unified Modern Infrastructure) may appear as the opposite sides of the moon. They are both key actors in the world of tools used by material science researchers but they couldn’t appear to be more further away.
Lumi is a petascale supercomputer located at the CSC data center in Kajaani, Finland. As of January 2023, the computer is the fastest supercomputer in Europe. Similarly FLASH is the world’s first Free Electronc Laser (FEL). It is part of the Desy Synchrotron and has provided extremely bright, coherent and ultra-short XUV pulses for a broad science programme conducted by scientists from all over the world since 2005.
In this talk I will discuss how the physics investigated in ultra–fast Pump & Probe experiments can connect Lumi and FLASH providing an unprecedent insight in the elemental processes occurring at the microscopic atomic scale on a ultra–short time–scale. I will review the novel Ab Initio Non Equilibrium Method (Ai–NEGF) and discuss how HPC resources can help in investigating regimes of matter and of theory, almost impossible to access using paper and pencil or a standard, even if large, Beowulf cluster.
I will describe the actual implementation of Ai–NEGF in the Yambo code discussing some recent numerical and methodological developments that have been implemented towards to exploitation of next generation HPC supercomputers. In particular, I will present the Yambo hybrid parallelization and I will also discuss the future plans of the project and its potential use as tool for science dissemination, also in third world countries.

- 16:10 - 16:30 - V. Pérez Carrasco, V. Lomüller, L. Sommer, J. Oppermann, R. Biessy, T. Ciglarič, and M. Goli. 
> 
\\
**Title**. Runtime Instantiation of Kernels for Fast Fourier Transforms Using SYCL Specialization Constants\\
\\
**Abstract**. In the domain of physics simulations, the pursuit of precision and scale exacerbates the need for additional compute power, for which heterogeneous systems have become an increasingly popular solution. SYCL (5), an industry defined, vendor-agnostic heterogeneous programming model implemented using standard C++, is a good candidate as a solution to write portable code that can fulfill the needs of highly demanding workloads. An important part of the SYCL ecosystem are libraries such as oneMKL (2), a mathematical kernel library, or portFFT (1), a SYCL library for Fast Fourier Transforms (FFTs), which not only provide performant building blocks, but also aid in developer productivity.\\
In this talk, we will give an overview of portFFT, leveraging SYCL to accelerate FFTs of different input sizes, which can be used in different physics applications, e.g. Gromacs (4). portFFT, as well as other similar libraries, balances binary size and performance for different FFT configurations. Ideally, we would like to have one highly optimized kernel for each possible input size generated at compile time, but this would greatly increase binary size, complicating deployment.\\
As a mitigation, SYCL introduces specialization constants, values which are guaranteed to stay constant throughout the execution of a kernel whose value can be set before kernel launch. SYCL implementations may use Just In Time (JIT) compilation to specialize kernels using the provided values before launch. This way, programmers can get the benefits of highly specialized kernels by instantiating them at runtime when the input sizes are already known. We show the results of applying this approach and a new Specialization Constant--Length Allocations (SCLA) extension (5) built on top of specialization constants.\\
Our modified version of the portFFT library using specialization constants and SCLA running a set of our tests reported a speedup compared to the original version using kernel execution time as a metric, demonstrating the potential of specialization constants for SYCL applications and libraries.

- 16:30 - 16:50 - M. Sander, H. Tröpgen, C. von Elm, and Schöne.
> 
\\
**Title**. Towards Large-scale Top-Down Microarchitecture Analysis Using the Score-P Framework\\
\\
**Abstract**. The Top-Down Microarchitecture Analysis Method introduced by Yasin established a simple yet effective generic approach to performance analysis. It can be used to analyze which microarchitectural resource poses a bottleneck during the execution of arbitrary codes. The recently introduced Golden Cove microarchitecture used in Intel’s Sapphire Rapids processors provides an extended, automated hardware support for this analysis. In this paper, we describe the implementation of this microarchitectural feature, integrate support into the performance measurement infrastructure Score-P, and explore the capabilities of the resulting tool with two example applications: The Computational Fluid Dynamics (CFD) solver for turbo-machinery applications Hydra, and the open-source weather and climate model ICON. 

- 16:50 - 17:30 - **Andrea Giordano - Keynote talk**: 
> 
\\
**Title**. A Survey on Cellular Automata Parallel Execution Techniques\\
\\
**Abstract**. Cellular Automata (CA) is a widely adopted paradigm for various physical systems, encompassing fluid dynamics, plasmas, spin systems, statistical mechanics, and natural phenomena such as lava flow, landslide, and prey-predator models. In each of these domains, CA modelling is able to capture the complexity of these systems by defining the interaction of their elementary units via relatively simple local rules. Due to an inherently parallel structure, CA executions can gain significant performance enhancements through parallel computing. In this talk, I will delve into the basic techniques for the parallel execution of CA on shared and distributed memory systems, as well as GPU architectures Moreover, I will explore optimization strategies, such as load balancing techniques, aimed at further amplifying the efficiency of parallel executions. In addition, I will introduce engineering practices geared towards facilitating transparent code execution. These practices aim to shield modellers from intricate computer science issues associated with execution contexts and optimization strategies, enabling them to focus solely on the modelling aspects of their work.

- 17:30 - 17:35 Closing notes

All times are in Central European Summer Time ([UTC+1](https://www.timeanddate.com/worldclock/spain/madrid)).

<!-- The complete EuroPar program is available at [https://2024.euro-par.org/program/](https://2024.euro-par.org/program/). 
-->

