Singularity image for AFL++ (https://github.com/AFLplusplus/AFLplusplus)

[![singularity-deploy](https://github.com/shub-fuzz/aflpp/actions/workflows/builder.yml/badge.svg?branch=main)](https://github.com/shub-fuzz/aflpp/actions/workflows/builder.yml)

- __What__ is [Singularity](https://sylabs.io/singularity/)??  
  A containerization system primarily used by the scientific community on high-performance computing (HPC).
  On many University HPC systems, docker is not allowed, but singularity is availble because it runs with 
  user level permisions.  
- __Why__?  
  Fuzzing on HPC!  
  Universities have trememdous resources available in HPC clusters that can be used to support 
  large-scale fuzzing evaluations.


- usage:

```
singularity pull --name aflpp.sif https://github.com/shub-fuzz/aflpp/releases/download/0.0.2/shub-fuzz-aflpp.1604.sif

singularity shell aflpp.sif
```

- pull Ubuntu 18.04 container

```shell
singularity pull --name aflpp.1804.sif https://github.com/shub-fuzz/aflpp/releases/download/0.0.2/shub-fuzz-aflpp.1804.sif
```
