# wkt
Weakly turbulent evolution of electrons, Langmuir waves and ion-sound waves in collisional plasma. The code was used to obtain results in  https://doi.org/10.1051/0004-6361/201118216 

WKT code (https://github.com/edkontar/wkt) starts with initial electron distribution as a beam 
The equations are modified to include a source of electrons 

$$f(v,t=0)=N_{beam}/(sqrt(2.\pi)*2*v_T) exp(-\frac{(v-20.v_T)^2}{2(2v_T)^2})$$

where the beam velocity is $20v_T$.

For details see also https://ui.adsabs.harvard.edu/abs/2002PhRvE..65f6408K/abstract


#### If not already installed on your system, download and install git for command line from https://git-scm.com/
#### Launch the Git Bash terminal
```bash
git clone https://github.com/edkontar/wkt wkt
cd wkt
git submodule update --init --recursive --remote
```
#### To compile with f95 compiler and build wkt binary 
```bash
f95 -o wkt constant.f90 params.f90 reader.f90 writer.f90 nonlins.f90 initbeam.f90 1beam.f90
```
