# LUDecomposition

Give permission to execute shell scripts:
    chmod 755 c_seq
    chmod 755 c_omp
    chmod 755 c_mpi
    chmod 755 r_seq
    chmod 755 r_omp
    chmod 755 r_mpi

**********************************************************************************************************
For the following commands, replace "size" by the matrix size that you want to test, and 
replace "nthreads" with the number of threads for OMP to execute with.

*For MPI, to change ntasks, edit mpi_slurm.sh, then run
    ./r_mpi size

Sequential:
    ./c_seq
    ./r_seq size

OpenMP:
    ./c_omp
    ./r_omp size nthreads

MPI:
    ./c_mpi
    ./r_mpi size

    to change ntasks, edit mpi_slurm.sh, then run
    ./r_mpi size