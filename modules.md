# Using modules in a cluster
Some, if not the majority of the supercomputing centers, install programs and make them available by modules. This is done specially so resource management programs could allocate computational tasks and run the programs without crashing the server (*e.g.* [PBS](https://www.pbspro.org/), [SLURM](https://slurm.schedmd.com/)). 

### Verify what modules are installed
First, cehck is the program (module) you need is already installed. Type:   
```bash
user@mycluster ~ $ module avail
```   
You will see are the programs currently available in the system.   
```
------------------------------------------------------------------------------------------------------------------
ansys/18.2           cfx/18.2           comsol/5.3a          fluent/19.1                gromacs/2016.3(default)  maple/2017                 matlab/R2017B_MCR         namd/2.9(default)         orca/4.0(default)       schrodinger/2018-1           wannier90/1.2(default)  
ansys/19.0           cfx/19.0           comsol/5.4(default)  fluent/19.2(default)       icem/19.0                maple/2018(default)        matlab/R2018A(default)    openfoam/v1706+           qespresso/6.1(default)  schrodinger/2018-3(default)  wannier90/2.0           
ansys/19.1           cfx/19.1           fluent/18.2          gamess/2018-02(default)    icem/19.1                mathematica/11.3(default)  matlab/R2018A_MCR         openfoam/v1806+(default)  R/3.3.2(default)        turbomole/7.3(default)       wien2k/17.1(default)    
ansys/19.2(default)  cfx/19.2(default)  fluent/19.0          gaussian/16.B.01(default)  icem/19.2(default)       matlab/R2017B              mscnastran/2018(default)  openfoam/v1806+_knl       schrodinger/2017-4      vasp/5.4(default)
```   
This is part of the output we get after running the command. As you can see we have many programs installed with their versions. In some cases we have a program with different version becasue you may have tools using old versions and do not suport new updates.
