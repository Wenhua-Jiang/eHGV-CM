# eHGV-CM: A Tool for Modelling the Charging of Electric Heavy-Goods Vehicles

In the context of modelling eHGV charging, understanding the requirements of the charging infrastructure is imperative for accurately capturing charging behaviour dynamics.These behaviours are influenced by factors like arrival patterns, charger availability, and the state of charge (SoC) upon arrival of trucks. In eHGV-CM, eHGVs are represented as individual agents in an agent-based model (ABM), each equipped with unique behaviours, preferences, and decision-making capabilities. Variables such as arrival battery state of charge (SoC) and time until the next mandated break have been integrated into the drivers' decision-making processes. This integration enables the simulation of scenarios wherein eHGVs dynamically adapt their charging behaviour in response to varying battery charge levels and imminent operational constraints. Moreover, this approach enables the depiction of real-world complexities, including diverse vehicle arrival times and charging demand patterns. 

The resulting level of granularity facilitates the exploration of complex interactions among eHGVs and charging infrastructures, thereby facilitating the identification of optimal charging strategies, infrastructure configurations, and policy interventions. 

By simulating these interactions within a virtual environment, we gain valuable insights into the impact of different charging infrastructure designs 
on system performance, efficiency, and overall sustainability. This will help policymakers, planners, and industry stakeholders make informed decisions 
and to optimise the deployment and operation of eHGV charging infrastructure as it starts to be rolled out nationally. Our current focus is on EU-specific 
vehicle availability and driver regulations, but the model is broadly generalisable to similar jurisdictions by altering a few key variables (such as the 
maximum driving time permitted before mandatory rest breaks or the potential maximum power of charging facilities).

# Installation

The simulation model is implemented in NetLogo. To run the model, please install NetLogo version 6.4 from https://ccl.northwestern.edu/netlogo/download.shtml. On Windows and macOS, you can launch NetLogo by double-clicking the application or the model file ./netlogo/vinos.nlogo, which will open the integrated development environment (IDE). On Linux, start NetLogo by running the netlogo-gui.sh shell script provided with the installation.


# Using the model

Upon opening the model, the truck arrival data (default_arrivals.csv) is loaded, and variables are initialized with their default values. The Interface tab of the IDE is displayed, featuring a hypothetical charging station with various types of chargers in the world view panel. Sliders and switches are available for adjusting parameters. When the "Go" button is clicked, the model advances, updating the view along with the plots.

The model allows for evaluating different charging station configurations. By default, the charging station is equipped with three types of chargers: ultra-fast chargers (1 MW), fast chargers (350 kW), and slow chargers (150 kW), with slow chargers primarily used for overnight charging. The quantities of each charger type can be adjusted using the sliders in the model. Additionally, you can modify the low and high battery thresholds, as well as the ratio of large trucks to small trucks. For more details about the model, please refer to the info tab.


# Evaluating a model simulation

The typical evaluation of a NetLogo model is visual inspection, as its canonical use is for education or participatory modeling. So go explore the changes in the view and the line and bar plots as you change parameters (a rising diesel price, perhaps?).

The model does write out geospatial data for later analysis with third-party GIS software in the directory ./netlogo/results/. Currently, static maps for water depth, accessibility, and OWF fraction are written out, as well as weekly maps of fishing effort and other dynamic variables. The output format is ESRII ASCII .asc raster data. Fleet statistical data is written out as ./netlogo/results/total_avg.csv comma-separated value tabular format.


# Contributing

We greatly appreciate your feedback, bug reports, and suggestions for improvement. To share your thoughts, simply open an issue on our repository. We also welcome your contributions!
The best way to contribute is by following these steps:

    (1) Forking our repository

    (2) Committing your changes to your fork

    (3) Creating a pull request (PR) to submit your changes back to us



