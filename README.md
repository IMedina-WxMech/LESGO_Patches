# LESGO_Patches
Modified Version of the JHU LESGO solver to accommodate roughness patches. 

## Primary changes:
* wallstress.f90: Within the ws_equilibrium_lbc subroutine, added loops to either explicitely add 2 patches with a set roughness ratio, length, and position or to add a .zip file of a roughness 'map'.
* lesgo.conf: Within the Solver Parameters section, added arguments for adding in 2 spanwise patches (with an explicit first patch roughness, roughness ratio, and patch lengths) and for the option of having a roughness map .zip file. This zip file MUST be in your lesgo folder, not the individual run folder. 
