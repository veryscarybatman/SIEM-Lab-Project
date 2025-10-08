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

# Configure data ingestion:

Install/configure lightweight log forwarders or use syslog/Windows Event Forwarding for sample hosts.

Define parsing/ingest pipelines (e.g., ECS/Elastic ingest pipelines or Splunk sourcetypes).

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
