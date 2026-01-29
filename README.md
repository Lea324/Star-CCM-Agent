## Star-CCM-Agent ##
---------------------------------------------------------------------------------------------------------------------------------
# Objective
This project aims to transform CFD workflows in Simcenter STAR-CCM+ from a manual, click-intensive process into a streamlined, AI-assisted pipeline, enabling engineers to focus on high-level physical modelling and design decisions rather than software syntax and repetitive operations.
The project develops an LLM-powered conversational agent that translates natural-language user instructions into executable Java macros for Simcenter STAR-CCM+. The agent assists with simulation setup, modification, and post-processing by generating and executing macros within the STAR-CCM+ environment under explicit user control.

---------------------------------------------------------------------------------------------------------------------------------
# Problem looking to be solved
A primary limitation in industrial CFD workflows is the manual interaction bottleneck. Engineers spend a disproportionate amount of time on repetitive and low-level tasks, including mesh configuration, physics setup, and the development and debugging of Java macros. In addition, effective monitoring of simulation health—such as interpreting association plots and residual convergence—requires continuous human oversight. This manual overhead slows the design iteration cycle and raises the barrier for non-experts to effectively utilise high-fidelity CFD tools such as Simcenter STAR-CCM+.

---------------------------------------------------------------------------------------------------------------------------------
# Technologies Used
Simcenter STAR-CCM+; LLM as the translator; STAR-CCM+ Java Macro API; Python / MATLAB as the monitor

---------------------------------------------------------------------------------------------------------------------------------
# Methodology
The agent operates as a human-in-the-loop, agent-assisted system. Natural-language user instructions are translated by the LLM into precise Java macros, which are executed within STAR-CCM+. During simulation execution, external Python or MATLAB scripts analyse solver outputs, including residual convergence histories and association plots.
Based on these diagnostics, the agent provides recommendations for parameter adjustments or workflow refinements, which can be applied automatically with user approval. This approach reduces manual monitoring effort, accelerates iteration cycles, and positions the simulation software as an intelligent assistant rather than a passive tool.
