HPL-MXP rules and validation
------------------------

The HPL-MXP benchmark is described at https://www.top500.org/project/linpack/.

When built from source, the HPL-MXP output shows the validity of the run on the following line:

.. code-block:: bash

   ||Ax-b||_oo/(eps*(||A||_oo*||x||_oo+||b||_oo)*N)=        0.0020152 ...... PASSED

The time output will look like the following for HPL-MXP:

.. code-block:: bash

   T/V                N    NB     P     Q               Time                 Gflops
   --------------------------------------------------------------------------------
   WR01C2L8      102144   192     8     8             514.92              1.380e+03

There is no minimum run time associated with HPL-MXP.

**Files to submit**

- HPL output saved to a file ``cert-{N}-mxphpl.rslts``
- HPL input file (``HPL.dat``) saved to a file ``cert-{N}-mxphpl.input``
- The script (or commands) used to run HPL saved to a file ``cert-{N}-mxphpl.run``
- HPL run timestamps saved to a file ``cert-{N}-mxphpl.tstamps``
- `Run configurations <https://scc24-benchmarking.readthedocs.io/en/latest/benchmarks/general.html#configuration-file-description>`_ saved to a file ``cert-{N}-configuration.txt``


