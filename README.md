# eHGV-CM: A Tool for Modelling the Charging of Electric Heavy-Goods Vehicles

When modeling eHGV charging, understanding the charging infrastructure is essential for capturing charging behavior. These behaviors are influenced by factors such as arrival patterns, charger availability, and the truck's state of charge (SoC) upon arrival. In eHGV-CM, eHGVs are represented as individual agents in an agent-based model (ABM), each with unique behaviors, preferences, and decision-making processes. Factors like battery state of charge and time until the next mandated break are integrated into the drivers' decision-making, allowing the model to simulate how eHGVs adjust their charging behavior based on battery levels and operational constraints. This approach also captures real-world complexities, like varying vehicle arrival times and charging demand patterns.

The model's level of detail enables exploration of interactions between eHGVs and charging infrastructure, helping identify optimal charging strategies, infrastructure configurations, and policy interventions.

Simulating these interactions in a virtual environment provides valuable insights into how different charging infrastructure designs impact system performance, efficiency, and sustainability. This helps policymakers, planners, and industry stakeholders make informed decisions to optimize eHGV charging infrastructure as it rolls out nationally. While the model focuses on EU-specific regulations and vehicle availability, it can be adapted to other regions by adjusting key variables, such as driving time limits or charger power capacity.

# Installation

The simulation model is implemented in NetLogo. To run the model, please install NetLogo version 6.4 from https://ccl.northwestern.edu/netlogo/download.shtml. On Windows and macOS, you can launch NetLogo by double-clicking the application or the model file ./netlogo/vinos.nlogo, which will open the integrated development environment (IDE). On Linux, start NetLogo by running the netlogo-gui.sh shell script provided with the installation.


# Using the model

Upon opening the model, the truck arrival data (default_arrivals.csv) is loaded, and variables are initialized with their default values. The Interface tab of the IDE is displayed, featuring a hypothetical charging station with various types of chargers in the world view panel. Sliders and switches are available for adjusting parameters. When the "Go" button is clicked, the model advances, updating the plots along with the monitors.

The model allows for evaluating different charging station configurations. By default, the charging station is equipped with three types of chargers: ultra-fast chargers (1 MW), fast chargers (350 kW), and slow chargers (150 kW), with slow chargers primarily used for overnight charging. The quantities of each charger type can be adjusted using the sliders in the model. Additionally, you can modify the low and high battery thresholds, as well as the ratio of large trucks to small trucks. For more details about the model, please refer to the info tab.


# Evaluating a model simulation

The typical evaluation of a NetLogo model relies on visual inspection, as it is primarily designed for participatory modeling. As you adjust parameters, explore how the plots and the monitors change in response.

By running the simulation with different configurations and settings, users can assess the effectiveness of various charging strategies, identify potential bottlenecks, and optimize the deployment of charging infrastructure. This evaluation helps reveal how factors such as charger availability and truck arrival patterns influence queue times, charging durations, and overall charging utilization efficiency.



# Contributing

We greatly appreciate your feedback, bug reports, and suggestions for improvement. To share your thoughts, simply open an issue on our repository. We also welcome your contributions!
The best way to contribute is by following these steps:

    (1) Forking our repository

    (2) Committing your changes to your fork

    (3) Creating a pull request (PR) to submit your changes back to us



