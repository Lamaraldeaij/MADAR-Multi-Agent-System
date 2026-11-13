# MADAR – Multi-Agent Satellite Mission Coordination System

## Project Description

MADAR is a Python-based multi-agent system designed to manage and coordinate satellite missions for Earth observation. The main goal of the project is to assign missions to suitable satellites and handle problems that may occur during execution, such as low battery levels, communication failures, and scheduling conflicts.

The system consists of six agents: Satellite Agent, Mission Agent, Ground Station Agent, Battery Agent, Communication Agent, and Coordinator Agent. Each agent has a specific role, and they work together to manage mission assignments, monitor satellite conditions, and reassign missions when needed.

MADAR also includes an interactive dashboard where users can adjust satellite battery levels, communication conditions, and mission priorities. Users can run different scenarios and monitor agent status, mission progress, and messages exchanged between agents. LangSmith is used to trace agent activities and evaluate the system's performance.

## Installation and Setup

To set up the MADAR project, follow these steps:

1. Download the project files from the GitHub repository.
2. Open the main notebook (Madar_1.ipynb) in Google Colab.
3. Install the required Python libraries listed in the requirements.txt file.
4. Configure your LangSmith API key securely to enable agent tracing.
5. Make sure the required project files, including MADAR.html, are available in the Colab environment.
6. Run the notebook setup cells to prepare the Python environment and start the backend server for the interactive dashboard.

Once the setup is complete, the system is ready to run. The next section explains how to launch the dashboard and use its features.

## Running the System

After completing the setup and opening the MADAR dashboard, follow these steps:

1. Select one of the available scenarios from the Quick Scenarios section, or customize the simulation settings.
2.Adjust the satellite battery levels, battery drain per step, ground link, battery threshold and mission priorities as needed.
3.Click the Run Simulation button to start the simulation. (Choosing a Quick Scenario runs it immediately; use Run Simulation after changing the settings manually.)
4. Monitor the simulation through the dashboard, where you can view satellite status, mission progress, agent activities, and communication messages.
5. Use the timeline controls to play, pause, move between simulation steps, and review important events.
6. Review the performance metrics and event logs to understand the system's results.

## Additional Instructions

- The system supports up to 5 missions per simulation.
- Battery levels must be between 0% and 100%.
- The battery threshold can be adjusted between 30% and 80%.
- With both satellites available, at least 3 missions are needed to create a scheduling conflict.
- The dashboard supports different scenarios, including Normal, Battery Drain, Link Loss, Conflict, Stress Test, and Total Blackout.
- Do not upload the LangSmith API key or other sensitive credentials to the public GitHub repository.
- The `MADAR.html` file can also run independently using its built-in simulation logic, but standalone runs are not traced in LangSmith.

