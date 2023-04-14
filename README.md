# wkt
Weakly turbulent evolution of electrons, Langmuir waves and ion-sound waves in collisional plasma. The code was used to obtain results in  https://doi.org/10.1051/0004-6361/201118216 

#### If not already installed on your system, download and install git for command line from https://git-scm.com/
#### Launch the Git Bash terminal
```bash
git clone https://github.com/edkontar/wkt wkt
cd wkt
git submodule update --init --recursive --remote
```
#### To compile with f95 compiler and build wkt binary 
```bash
f95 -O3 -o wkt constant.f90 params.f90 reader.f90 writer.f90 nonlins.f90 initbeam.f90 1beam.f90
```
