# MagnePlane (Hyperloop_v2)

"It's more of a plane without wings, than a train without wheels"

Expanding upon previous work

https://github.com/jcchin/hyperloop/tree/scitech

https://github.com/narwhaltribe/Hyperloop

Apache V2 License

========

Dev forks can be found here:

[Chris Heath](https://github.com/cmheath/MagnePlane)

[Jeff Chin](https://github.com/jcchin/MagnePlane)

[Ken Moore](https://github.com/Kenneth-T-Moore/MagnePlane)

========
### File Structure

* AFLR3 - Advancing Front Local Reconnection viscous meshing software
  * Hyperloop.aflr3.arg - Output arguments file for aflr3
  * Hyperloop.tags - Grid boundary conditions tagging file for Magneplane geometry model
  * Hyperloop_PW.mapbc - Flow solver boundary condition mapping file for Magneplane geometry model
* ESP - Engineering SketchPad geometry tool developed by MIT/Syracuse University
  * capsule.csm - Geometry input build script file
  * capsule.udc
  * flow_domain.csm
  * tube.udc
* Fun3D - Aerodynamic flow solver
  * Hyperloop.mapbc
  * fun3d.nml
  * fun3d.template - Fun3D template file 
  * qscript - Sample portable batch system (PBS) queing script to run aero simulation on Pleiades (NASA's Advanced Supercomputer)
* Pointwise - 
  * Hyperloop-Mesher.glf - Sample Pointwise viscous meshing script for Magneplane vehicle
  * Hyperloop.mapbc - 
  * Hyperloop.pw - Sample Pointwise generated surface grid
* Geometry -
  * csm
    * hyperloop.csm
    * hyperloop2.csm
    * inlet_test.csm
  * Hyperloop.SLDPRT
* Python - 
  * LIM.py - Linear Induction Motor Calcs [Not Started]
  * aero.py - Fun 3d Wrapper
  * aflr3.py - AFLR External Code Wrapper
  * aflr3.script - Shell Meshing Script
  * air_bearing.py - Basic Air Bearing Calcs [Deprecate]
  * api.py - Defined python imports
  * battery.py - Battery Calculations
  * cycle.py - Re-write of NPSS cycle in Pycycle
  * cycle_wrapper.py - Python File wrap around NPSS
  * inlet.py - Calculates the dimensions for the inlet and compressor entrance
  * levitation.py - Halbach Array Lift/Drag Calculations
  * mass.py - Vehicle Mass estimations
  * mission.py - Extremely Basic Mission Calcs [to be replaced]
  * pax_cabin.py - passenger cabin sizing
  * pod.py - Vehicle Assembly
  * tube_cost.py - Port of Tom Gregory's initial cost calculations
  * tube_limit_flow.py - Isentropic flow relations for determining flow speed around pod
  * tube_structure.py - Tube structural calcs [Placeholder]
  * tube_wall_temp.py - Calculates steady state temperature within the tube
  * vacuum.py - Vacuum Pump calculations
  * tests - test scripts
    * test_cycle.py - unit tests for pycycle `cycle.py` model
    * test_temp.py - unit tests for `tube_wall_temp.py`
* NPSS - Numerical Propulsion System Simulation (Thermodynamic Cycle Analysis Tool)
  * area.view_page - "Viewer" file defining output
  * magneplane.mdl - Actual cycle model
