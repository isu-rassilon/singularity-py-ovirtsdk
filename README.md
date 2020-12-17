# oVirt Python SDK in a Singularity Container
This repository contains a Singularity definiton file which creates a container with the oVirt Python SDK in it.

To use:

1. clone the repository or download the Singularity definition file (py-ovirtsdk.def).

2. cd into the directory with the Singularity definition file.

3. run: sudo singularity build py-ovirtsdk.sif py-ovirtsdk.def

4. when done, any user can use the container via 'singularity run py-ovirtsdk.sif bash' or whatever.
