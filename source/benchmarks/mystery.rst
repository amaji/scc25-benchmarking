Mystery benchmark rules and validation
--------------------------------------

This year, we will use the `NAS Parallel Benchmarks (NPB) <https://www.nas.nasa.gov/software/npb.html>`_ as the mystery benchmark. More specifically, teams are required to run the ``CG`` and ``MG`` kernels from the NPB suite across a selection of problem sizes and plot their runtimes. Follow the steps described below to submit your NPB results to the SCC committee. Teams are requested to read the detailed descriptions about the benchmarks and how to run them from the `NPB website <https://www.nas.nasa.gov/software/npb.html>`_.

**Steps**

- Download the NAS parallel benchmarks (NPB) from the `NPB website <https://www.nas.nasa.gov/software/npb.html>`_. You must download the MPI version of the benchmark: ``NPB3.4.3.tar.gz``. After unpacking use the MPI version (``NPB3.4-MPI``).
- Compile the benchmark with your preferred compiler and MPI library. You can use any package manager such as spack or easybuild to compile the benchmarks.
- Run the kernels ``CG``, and ``MG`` for the problem classes ``B``, ``C``, ``D``, and ``E``.
- You must run the benchmarks across 2 or more nodes.
- Plot the run times of both the benchmarks across the problem classes, i.e., problem sizes.
- Write a brief report (`no more than 1 page`) describing the following:
   - How did you compile the benchmark?
   - Did you do any tuning to reduce the runtimes? 
   - How did you tune your benchmark runs?
   - How do the runtimes grow with increasing problem size?
   - Plot the run times for the CG and MG kernels across problem classes. 

**Submission instructions**

When the NPB benchmark runs successfully, it will generate an output file with lines like these:

.. code-block:: bash

 Benchmark completed
 VERIFICATION SUCCESSFUL
 Zeta is     0.7752216459940E+02
 Error is    0.1805637389876E-12 


 CG Benchmark Completed.
 Class           =                        E
 Size            =                  9000000
 Iterations      =                      100
 Time in seconds =                   XXX.XX
 

We will look at both the "VERIFICATION" line and the "Time in seconds".

Please submit the following files for the NPB benchmark.

- NPB output saved to a file ``cert-{N}-npb.rslts``. If you have multiple result files, combine them into a single file.
- NPB build script saved to a file ``cert-{N}-npb.build``.
- The script (or commands) used to run NPB saved to a file ``cert-{N}-npb.run``.
- NPB run timestamps saved to a file ``cert-{N}-npb.tstamps``.
- Report of the NPB run described in the previous section.

**Hints**

- You may need to create the file ``config/make.def`` from the provided templates before compiling.
- Do not use parallel builds (``-j NN``) when compiling the kernels.


