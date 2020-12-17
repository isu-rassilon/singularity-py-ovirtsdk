# singularity-py-ovirtsdk
A singularity file that installs CentOS 8 and the oVirt Python SDK.

To use:

1. clone the repository or download the Singularity definition file.

2. cd into the directory with the Singularity definition file.

3. run: sudo singularity build py-ovirtsdk.sif Singularity

4. when done, any user can use the container via 'singularity run py-ovirtsdk.sif bash' or whatever.
