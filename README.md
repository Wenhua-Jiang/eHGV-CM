# eHGV-CM: A Tool for Modelling the Charging of Electric Heavy-Goods Vehicles

In the context of modelling eHGV charging, understanding the requirements of the charging infrastructure is imperative for accurately capturing charging behaviour dynamics.These behaviours are influenced by factors like arrival patterns, charger availability, and the state of charge (SoC) upon arrival of trucks. In eHGV-CM, eHGVs are represented as individual agents in an agent-based model (ABM), each equipped with unique behaviours, preferences, and decision-making capabilities. Variables such as arrival battery state of charge (SoC) and time until the next mandated break have been integrated into the drivers' decision-making processes. This integration enables the simulation of scenarios wherein eHGVs dynamically adapt their charging behaviour in response to varying battery charge levels and imminent operational constraints. Moreover, this approach enables the depiction of real-world complexities, including diverse vehicle arrival times and charging demand patterns. 

The resulting level of granularity facilitates the exploration of complex interactions among eHGVs and charging infrastructures, thereby facilitating the identification of optimal charging strategies, infrastructure configurations, and policy interventions. 

By simulating these interactions within a virtual environment, we gain valuable insights into the impact of different charging infrastructure designs 
on system performance, efficiency, and overall sustainability. This will help policymakers, planners, and industry stakeholders make informed decisions 
and to optimise the deployment and operation of eHGV charging infrastructure as it starts to be rolled out nationally. Our current focus is on EU-specific 
vehicle availability and driver regulations, but the model is broadly generalisable to similar jurisdictions by altering a few key variables (such as the 
maximum driving time permitted before mandatory rest breaks or the potential maximum power of charging facilities).


# Installation

The simulation model is implemented in NetLogo. To run the model, please install NetLogo version 6.4 from https://ccl.northwestern.edu/netlogo/download.shtml. On Windows and macOS, you can open NetLogo by double-clicking the application or the model file ./netlogo/vinos.nlogo, which will launch the integrated development environment (IDE). On Linux, start NetLogo with the netlogo-gui.sh shell script provided by NetLogo.


# Using the model

Upon opening the model, all data are loaded, variables are initialized with default values and the Interface tab of the IDE is shown, with a North Sea map displayed in the world view panel, and sliders and switches to change parameters. Upon clicking the go button, the model advances and the view as well as the line and bar plots are updated.

