# MPCC
This is a Matlab implementation of the MPCC controller. The implementation is very similar to the approach descriebed in [Optimization‐based autonomous racing of 1:43 scale RC cars](https://onlinelibrary.wiley.com/doi/abs/10.1002/oca.2123). 

## How to run

The simplest way to run the code is using the quadprog interface as this needs no dependencies. However, we recomand the hpipm interface as it reduces the solve times massivly which makes working with the simulation more convininat.

### Before running code
1) Install [hpipm](https://github.com/giaf/hpipm) including the Matlab mex interface
2) alternatively install Yalmip or CVX, or use the quadprog interface
### Run code
0) in simulation.m change to the optimization framework you use (hpipm, Yalmip, CVX, quadprog)
1) run simulation.m
2) play with the tunning in getMPC_vars.m
3) change the car model between FullSize and ORCA
4) change the track layout between the ORCA and the RCP track

### Notes
1) If you use the RCP track the obstacle postions need to be changed by hand

## Options
Beside the 1:43 RC cars, we also implemented a full sized car model as well as two possible tracks.