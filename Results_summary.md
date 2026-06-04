# Results Summary

## Project Overview

This project evaluated the effectiveness of an AI-assisted Security Operations Center (SOC) triage system compared to human SOC analysts. The environment was built using Wazuh, OpenSearch, Filebeat, Docker Compose, Oracle Cloud Infrastructure, and a custom AI triage container integrated with the OpenAI API.

The study measured:

* Triage accuracy
* Misclassification rates
* Incident consolidation
* Response efficiency
* Human versus AI decision making

---

## Scenario 1: SSH Brute Force Attack

* Approximately 4,700 authentication failure alerts generated.
* AI processed the full alert stream and generated 3,098 separate incidents.
* Human analysts correctly identified the activity as a single brute-force campaign.
* AI demonstrated rapid processing but poor incident consolidation.

### Key Finding

Human analysts successfully recognized attack patterns and grouped related alerts into one incident, while AI fragmented the activity into thousands of separate incidents.

---

## Scenario 2: Sudo Privilege Escalation

* Approximately 17,797 alerts generated.
* AI produced 446 incidents.
* Human analysts correctly identified the activity as a single privilege escalation campaign.
* AI recognized elevated severity but lacked contextual understanding.

### Key Finding

Human analysts connected multiple related events into a coherent attack sequence. AI identified suspicious activity but over-segmented the data.

---

## Scenario 3: File Integrity Tampering

* 24 malicious alerts generated.
* AI produced zero incidents.
* Human analysts correctly identified and escalated the attack.

### Key Finding

This scenario resulted in a critical false negative for the AI system. Despite successful alert ingestion, the model failed to classify any malicious activity.

---

## Overall Findings

### AI Strengths

* Extremely fast processing
* Effective handling of high alert volumes
* Consistent output generation
* Useful for reducing manual review workload

### AI Weaknesses

* Poor incident consolidation
* Limited contextual awareness
* Weak campaign-level reasoning
* Critical failure in low-volume, high-severity scenarios

### Human Analyst Strengths

* Strong contextual interpretation
* Accurate incident consolidation
* Superior attack pattern recognition
* Reliable escalation decisions

### Conclusion

The results support a hybrid SOC model in which AI assists analysts by processing large alert volumes while human analysts provide contextual reasoning, incident correlation, and final decision making.
