# Parallel algorithm to generate Mandelbrot fractals using MPI 

Project for the course of Advanced Computing from Instituto Politécnico de Bragança (IPB), this project applies parallel computing using MPI to a serial code for the generation of the Mandelbrot set. 

The instructions and requirements for this project are described in the file [practical-work.pdf](https://github.com/XavierJece/Mandelbrot-with-MPI/blob/main/practical-work.pdf).

1. **Create the executable files:**
    - Enter the ac-mandelbrot-resources folder: `cd ac-mandelbrot-resources` 
    - The makefile has two different commands
    - `make` will generate the *.exe* file for serial version
    - `make mpi` will generate the *.exe* file for the MPI version

1. **Execute the program**
    - Serial version command: `./mandelbrot-gui-serial.exe`
    - MPI version command: `mpirun -np <number_of_workers> --hostfile localhost.OPENMPI ./mandelbrot-gui-mpi.exe`
        - For the MPI version you can change the number of workers used by changing the number that comes after `-np`
