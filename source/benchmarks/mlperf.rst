MLPerf rules and validation
---------------------------

The instructions to run the MLPerf-SDXL inference benchmark and submit your results 
can be found in `this tutorial <https://docs.mlcommons.org/inference/benchmarks/text_to_image/reproducibility/scc24/>`_. MLPerf results must be uploaded to the ``cm4mlperf-inference`` repository as described in the `tutorial <https://docs.mlcommons.org/inference/benchmarks/text_to_image/reproducibility/scc24/>`_.

**Things to remember**

  - Note that MLPerf writes both to `stdout` and `stderr` - you will need to capture both streams for your submission.
  - Teams are encouraged to download the latest copy of the MLPerf-SDXL codes at the competition. This will make sure that your runs incorporate latest features and bug fixes in the benchmark.
  - If your team made modifications to be MLPerf codes, such code changes must be shared with the SCC24 committee by Nov 13, 2024 (Wed). Failure to submit the code changes by this deadline will invalidate your results.
  - Teams that make significant community contributions may be awarded bonus points at the discretion of the SCC24 committee. To receive bonus points, teams must 1) publicly share their code changes with the community by creating a pull request to the ``cm4mlops`` repository at least 48 hours before the start of the competition (Nov 16, 2024, 9:00AM EDT), 2) have their code changes reviewed by the MLCommons reviewer(s), 3) accept the Contributor License Agreement (CLA) to merge the PR into the repository.
