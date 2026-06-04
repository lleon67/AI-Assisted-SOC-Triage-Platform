# AI-Assisted-SOC-Triage-Platform
AI-assisted SOC triage platform using Wazuh, OpenSearch, Docker, and OpenAI to compare human and AI analyst performance in simulated attack scenarios.


This project evaluates the accuracy, efficiency, and limitations of AI-assisted Security Operations Center triage compared to human SOC analysts. The environment was built using Wazuh, OpenSearch, Filebeat, Docker Compose, Oracle Cloud Infrastructure, and a custom AI triage container integrated with the OpenAI API.

The study tested three simulated attack scenarios: SSH brute force, sudo privilege escalation, and file integrity tampering. Results showed that AI processed alerts quickly but struggled with incident consolidation and failed entirely in one low-volume, high-severity scenario. Human analysts were slower, but demonstrated stronger contextual reasoning, pattern recognition, and incident consolidation.
