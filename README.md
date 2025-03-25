# eHGV-CM: A Tool for Modelling the Charging of Electric Heavy-Goods Vehicles

In the context of modelling eHGV charging, understanding the requirements of the charging infrastructure is imperative for accurately capturing charging behaviour dynamics. These behaviors are influenced by factors such as arrival patterns, charger availability, and the truck's state of charge (SoC) upon arrival. In eHGV-CM, eHGVs are represented as individual agents in an agent-based model (ABM), each with unique behaviors, preferences, and decision-making processes. Factors like battery state of charge and time until the next mandated break are integrated into the drivers' decision-making, allowing the model to simulate how eHGVs adjust their charging behavior based on battery levels and operational constraints. This approach also captures real-world complexities, like varying vehicle arrival times and charging demand patterns. The resulting level of granularity facilitates the exploration of complex interactions among eHGVs and charging infrastructures,  helping identify optimal charging strategies, infrastructure configurations, and policy interventions.

Simulating these interactions in a virtual environment provides valuable insights into how different charging infrastructure designs impact system performance, efficiency, and sustainability. This helps policymakers, planners, and industry stakeholders make informed decisions to optimize eHGV charging infrastructure as it rolls out nationally. While the model focuses on EU-specific regulations and vehicle availability, it can be adapted to other regions by adjusting key variables, such as driving time limits or charger power capacity.

# Installation

The simulation model is implemented in NetLogo. To run the model, please install NetLogo version 6.4 from https://ccl.northwestern.edu/netlogo/download.shtml. On Windows and macOS, you can launch NetLogo by double-clicking the application or the model file ./netlogo/vinos.nlogo, which will open the integrated development environment (IDE). On Linux, start NetLogo by running the netlogo-gui.sh shell script provided with the installation.


# Using the model

Upon opening the model, the truck arrival data (default_arrivals.csv) is loaded, and variables are initialized with their default values. The Interface tab of the IDE is displayed, showcasing a hypothetical charging station with various charger types in the world view panel. Sliders and switches are provided to adjust parameters. When the "Go" button is clicked, the model advances, updating the plots and displaying key output metrics on the monitors.

The model allows for evaluating different charging station configurations. By default, the charging station is equipped with three types of chargers: ultra-fast chargers, fast chargers, and slow chargers, with slow chargers primarily used for overnight charging. The quantities of each charger type can be adjusted using the sliders in the model. Additionally, you can modify the low and high battery thresholds, as well as the ratio of large trucks to small trucks. For more details about the model, please refer to the Info tab in the NetLogo graphical interface.


# Evaluating the model simulation

NetLogo models are typically assessed through visual inspection, as they are designed for interactive simulations and participatory modeling. The model's behavior can be evaluated by adjusting parameters and observing how plots and monitors respond to changes.

By running the simulation with different parameter configurations, users can evaluate how factors such as charger availability impact the number of queued trucks, queue times, charging durations, and overall charging utilization efficiency.


# Contributing

We greatly appreciate your feedback, bug reports, and suggestions for improvement. To share your thoughts, simply open an issue on our repository. We also welcome your contributions!
The best way to contribute is by following these steps:

    (1) Forking our repository

    (2) Committing your changes to your fork

    (3) Creating a pull request (PR) to submit your changes back to us



