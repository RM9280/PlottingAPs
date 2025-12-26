This project implements a biophysically realistic axon fiber simulation using a multi-compartment Hodgkin–Huxley model.
It recreates the default “Fiber” simulation from anctoolkit.com, combining:

Intracellular stimulation, 
extracellular stimulation, 
axial (internodal) current coupling, 
multi-node action potential propagation, 
swing-based visualization

The simulation models 10 nodes of Ranvier, computes membrane potentials over time, detects action potentials, and visualizes spike timing across nodes.

| Parameter              | Value    |
| ---------------------- | -------- |
| Time step (`dt`)       | 0.001 ms |
| Total duration         | 100 ms   |
| Intracellular stimulus | +10      |
| Extracellular stimulus | −700     |
| Stimulus duration      | 0.1 ms   |
| Stimulus delay         | 34 ms    |
| Nodes simulated        | 10       |

**For each node:**

AP start detected when voltage crosses above 0 mV

AP end detected when voltage falls below 0 mV

anctoolkit.com for the original fiber simulation concept
Chris Fietkiewicz and Albright Dwarka (HWS ’21)
SwingGraphics originally written by Ian Waldschmidt (Case Western Reserve University)
