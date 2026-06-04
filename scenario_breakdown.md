# Attack Scenario Breakdown

## Scenario 1: SSH Brute Force Attack

### Objective

Simulate repeated authentication failures against nonexistent user accounts.

### Detection Rule

* Wazuh Rule 5710

### Alert Volume

* Approximately 4,700 alerts

### AI Outcome

* 3,098 incidents generated
* Successfully identified malicious activity
* Failed to consolidate related alerts

### Human Outcome

* All analysts identified a single brute-force campaign
* Consistent escalation decisions
* Strong attack pattern recognition

### Key Takeaway

AI detected suspicious behavior but fragmented the activity into thousands of incidents. Human analysts correctly identified a single coordinated attack.

---

## Scenario 2: Sudo Privilege Escalation

### Objective

Simulate privilege escalation activity through repeated sudo commands.

### Detection Rule

* Wazuh Rule 5402

### Alert Volume

* Approximately 17,797 alerts

### AI Outcome

* 446 incidents generated
* Moderate severity scoring
* Limited contextual understanding

### Human Outcome

* Analysts identified a single privilege escalation campaign
* Successfully connected related events
* Correctly escalated malicious activity

### Key Takeaway

Human analysts demonstrated superior contextual awareness and campaign-level reasoning.

---

## Scenario 3: File Integrity Monitoring Tampering

### Objective

Simulate unauthorized modifications to monitored system configuration files.

### Detection Rule

* Wazuh Rule 554

### Alert Volume

* 24 alerts

### AI Outcome

* Zero incidents generated
* Complete classification failure
* Critical false negative

### Human Outcome

* Correctly identified malicious activity
* Escalated all relevant events
* Recommended containment actions

### Key Takeaway

This scenario exposed a significant limitation in AI-assisted SOC triage. Human analysts immediately recognized malicious activity while the AI system failed to produce any classification.

---

## Final Observation

Across all scenarios, AI demonstrated exceptional processing speed but struggled with contextual understanding and incident correlation. Human analysts consistently produced more accurate and meaningful incident assessments, supporting the use of AI as a SOC augmentation tool rather than a replacement for human expertise.
