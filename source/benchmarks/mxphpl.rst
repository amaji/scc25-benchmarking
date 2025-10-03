HPL-MXP rules and validation
------------------------

The HPL Mixed Precision (HPL-MXP) benchmark is described at https://hpl-mxp.org/.

Different vendors provide optimized implementation of the HPL-MXP benchmarks and teams are encouraged to use these vendor-optimized implementations to get the maximum performance on their clusters.

Nvidia HPL-MXP implementation: https://docs.nvidia.com/nvidia-hpc-benchmarks/HPL_MxP_benchmark.html
AMD HPL-MXP implementation: https://www.amd.com/en/developer/resources/infinity-hub/hpl-mxp.html

The HPL-MXP output shows the validity of the run on the following line:

.. code-block:: bash

   ||Ax-b||_oo/(eps*(||A||_oo*||x||_oo+||b||_oo)*N)=        0.0020152 ...... PASSED

The time output will look like the following for HPL-MXP:

.. code-block:: bash

   T/V                N    NB     P     Q               Time                 Gflops
   --------------------------------------------------------------------------------
   WR01C2L8      102144   192     8     8             514.92              1.380e+03

There is no minimum run time associated with HPL-MXP.

**Files to submit**

- HPL-MXP output saved to a file ``cert-{N}-mxphpl.rslts``
- HPL-MXP input parameters saved to a file ``cert-{N}-mxphpl.input``
- The script (or commands) used to run HPL-MXP saved to a file ``cert-{N}-mxphpl.run``
- HPL-MXP run timestamps saved to a file ``cert-{N}-mxphpl.tstamps``

