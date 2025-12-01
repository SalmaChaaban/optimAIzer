# ------------------------ OptimAIzer ------------------------


# 🧠 Problem Statement

Working on a computer can sometimes become stressful and overwhelming, as modern computers, though advanced, generate thousands of data points every second from CPU load, memory consumption, and more. Many user (technical and non-technical) may not understand these metrics or have the time to constantly troubleshoot what is slowing their computer down.

OptimAIzer addresses this challenge by using AI Agents to turn raw system data into an intelligent, human-friendly dashboard, providing actionable recommendations or automated fixed based on your own system's needs.


# 💡 Solution Overview

OptimAIzer is an AI-powered system monitoring and optimizing agent that:
- Collects system metrics via Python
- Processes and evaluates system health in real-time
- Generates a clean, readable report
- Recommends actions/automated fixes based on intelligent rule-based and LLM-assisted reasoning

This project applied course concepts, including:
- Agent workflows
- Tool calling (and creation)
- Context Engineering
- Reasoning + rule-based agents
- Multi-agent orchestration


# 🧩 Architecture
Components:
- Monitor agent: Collects the system metrics (CPU, memory, etc.)

- Analyzer agent: Analyzes the metrics collected by the monitor agent

- Autofix agent: Fixes issues based on the analysis

## 🔄 Flow
            
        [System Metrics] 
                |
                v
        [Monitor Agent] --(raw metrics)--> [Analyzer Agent] 
                |                                 |
                |                                 v
                |                         [Issues & Severity]
                |                                 |
                v                                 v
        [Structured Data / Flags] --------> [Autofix Agent]
                                                  |
                                                  v
                                       [Recommendations & Fixes]
                                                  |
                                                  v
                                          [Report Generator]
                                                  |
                                                  v
                                             [User Report]


# 🎯 Conclusion

OptimAIzer is an AI Agent system designed to help users optimize performance-related workflows by collecting and analyzing data, then generating actionable recommendations or applying them. The project demonstrates the practical application of key concepts from the course and leverages a multi-agent architecture, where separate agents handle data ingestion, analysis, and optimization tasks.

The agents are created using Google's ADK toolkit and are powered by a large language model (Gemini). They leverage both built-in tools and custom logic for domain-specific tasks, such as cross-platform system optimization. Users can view system insights of their system and improvement recommendations through the notebook's output and optionally apply automated fixes.


## 📈 Roadmap

While functional, this project has room for improvement, which may include:
- A dedicated, intuitive user interface
- Customizable reports tailored to user preferences
- More advanced and dynamic auto-fix capabilities


# ⚙️ Setup Instructions

1. Install Python

2. Clone or Download the Project from the GitHub repository: git clone https://github.com/SalmaChaaban/optimAIzer.git

3. Open the project in a code editor (e.g. VS Code)

4. Install Required Packages (packages are in the requirement.txt file, with the installation command in the notebook, at the top)

5. Add your GOOGLE_API_KEY to the .env file

6. Run the notebook (either cell by cell or all at once)


## Output Report Preview

![Output Report Preview](output_report.png)

(Outputs have been removed from the repository for privacy)
