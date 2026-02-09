## Auto Scaling Insight

A single EC2 instance is a single point of failure.

By placing instances inside an Auto Scaling Group and automating configuration with user data, the system becomes self-healing.

Instances are treated as disposable resources. If one fails, it is automatically replaced with an identical server, ensuring consistent service availability.

This architecture removes manual recovery and reduces downtime.
