

## Calculate area of Mandlebrot in parallel by OpemMP and MPI.

mpicc -> sudo apt-get install libopenmpi-dev
### To run only openMP file
- Compile with fopenmp flag
```
    mpicc OpenMpVersion.c -o mp -fopenmp
```
- Run
```
    ./mp
```

### To run only MPI file
- Compile with mpicc compiler
```
    mpicc MPIVersion.c -o mpi
```

- Run 
```
    mpirun -np <# of processes per node> mpi
```

### To run only openMP/MPI file
- Compile with mpicc compiler
```
    mpicc MPIOpenMPVersion.c -o mpiopenmp -fopenmp
```

- Run 
```
    mpirun -np <# of processes per node> mpiopenmp
```
