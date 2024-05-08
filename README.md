# MPC-matlab
## Gain-Scheduled MPC Control of Nonlinear Chemical Reactor
**About the Continuous Stirred Tank Reactor**
<p>A continuously stirred tank reactor (CSTR) is a common chemical system in the process industry. A schematic of the CSTR system is:</p>

<p align="center"><img width="50%" src="/image/image.png"></p>
<p>This system is a jacketed non-adiabatic tank reactor described extensively in [1]. The vessel is assumed to be perfectly mixed, and a single first-order exothermic and irreversible reaction, A --> B, takes place. The inlet stream of reagent A is fed to the tank at a constant volumetric rate. The product stream exits continuously at the same volumetric rate, and liquid density is constant. Thus, the volume of reacting liquid is constant.</p>

| The inputs of the CSTR model are:         | The outputs of the model, which are also the model states, are:    |    
| ----------------------------------------  | ------------------------------------------------------------------ |
|                                           |                                                                    |
| ![alt text](/image/image-1.png)           | ![alt text](/image/image-2.png)                                                                   |

- [Gain-Scheduled MPC Control of Nonlinear Chemical Reactor](</Gain-Scheduled MPC Control of Nonlinear Chemical Reactor/Gain-Scheduled MPC Control of Nonlinear Chemical Reactor.pdf>)
1. MPC single sim(mpc_mdl,10) / T=10
   
<p align="center"><img width="50%" src="/image/10.png"></p>

2. MPC single sim(mpc_mdl,60) / T= 60
<p align="center"><img width="50%" src="/image/60.png"></p>

3. MPC Multiple sim(mmpc_mdl), T=60

<p align="center"><img width="50%" src="/image/MMPC.png"></p>
<p>References: </p>
[1] Seborg, D. E., T. F. Edgar, and D. A. Mellichamp, Process Dynamics and Control, 2nd Edition, Wiley, 2004.

