# SIEM-Lab-Project
A self-contained lab for learning SIEM deployment, log ingestion, detection tuning, and incident response workflow. Intended for defensive training (blue team) and SOC skill-building.
Objective: to create an active SIEM and demonstrate its logging and alerting capability. 

# Choose SIEM solution:

This project uses Huntress (Free Trial)

# Prepare lab infrastructure:

Create an isolated network/virtual environment for SIEM components and test system.
we will be using Ubuntu in a VirtualBox VM.
# Provision SIEM components:

Deploy indexer/storage, search/query UI, and log forwarding/collector components (agent/forwarder endpoints).

# Configure 2 VMs. One for the SIEM, and one that will function as the attack vector. 

We will have VirtualBox installed so it can host both VMs. Download 2 VMS. This case will use Ubuntu for the SIEM and Kali for the attack vector. 

# Normalize and enrich:

Map fields to a consistent schema, add host metadata (hostnames, tags), and enrichment (asset owners, geoIP) where helpful.

# Implement detections and correlation:

Add a small set of baseline detection rules (suspicious login rate, unusual process execution patterns) — keep rules high level and generic.

# Create dashboards and visualizations:

Build dashboards showing ingestion volume, host activity, and detection alerts.

# Alerting and workflow:

Configure alert notifications (email/webhook) and an incident logbook to track simulated detections.

# Retention and archiving:

Configure indices/retention policies and document storage costs for longer retention.

# Test and validate:

Generate safe, authorized test events (synthetic logs, benign scripts that emit logs) to validate parsing and detections.

# Conclusion
