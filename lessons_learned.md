# Lessons Learned

This project provided practical experience in deploying, troubleshooting, and evaluating an AI-assisted Security Operations Center environment.

## Infrastructure Challenges

Building a functional SOC environment required significantly more effort than expected. Major challenges included:

* TLS certificate configuration failures
* OpenSearch authentication issues
* Missing environment variables
* Docker container communication problems
* Cloudflare tunnel failures
* SSH port forwarding configuration
* Dashboard access troubleshooting

These challenges reinforced the importance of infrastructure reliability within security operations environments.

---

## AI Security Insights

One of the most important discoveries was that AI performance is highly dependent on context and data characteristics.

While the AI system successfully processed large volumes of alerts, it struggled to:

* Correlate related events
* Identify campaign-level activity
* Understand attacker intent
* Recognize low-volume but high-severity incidents

The complete failure to classify the File Integrity Monitoring scenario demonstrated that AI systems should not be trusted without human oversight.

---

## Human Versus AI

Human analysts consistently demonstrated:

* Better contextual reasoning
* Stronger pattern recognition
* More accurate incident consolidation
* Better understanding of attacker behavior

AI excelled in speed and scalability but lacked the decision-making depth required for independent SOC triage.

---

## Security Engineering Experience

This project provided hands-on experience with:

* Wazuh deployment
* OpenSearch administration
* Docker Compose environments
* Linux troubleshooting
* Cloud infrastructure
* Security monitoring pipelines
* AI-assisted security workflows

The deployment process highlighted how operational challenges can directly impact security visibility and incident response effectiveness.

---

## Future Improvements

Future iterations of this project could include:

* SOC-specific model fine tuning
* Improved event correlation logic
* Expanded analyst participation
* Real-time analyst review workflows
* Automated infrastructure deployment through Infrastructure-as-Code
* Enhanced AI explainability and decision transparency

The project ultimately demonstrated that AI can enhance SOC operations but cannot currently replace human analysts for contextual decision making and incident analysis.
