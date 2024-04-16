The Horizontal Pod Autoscaler automatically adjusts the number of pods in a deployment, replica set, or [[Replication Controller]] based on observed CPU utilization or other selected metrics.
- **Mechanism:**
    - HPA fetches metrics from a series of aggregated APIs like metrics.k8s.io, custom.metrics.k8s.io, and external.metrics.k8s.io.
    - It adjusts the number of replicas automatically to maintain the target metric value (like CPU usage), defined in the HPA configuration.
- **Configuration:**
    - An HPA configuration includes the definition of the minimum and maximum number of pods, the target type (e.g., CPU utilization), and the target value for that metric.
- **Benefits:**
    - Provides dynamic scaling of applications according to their demand, thereby optimizing resource utilization and maintaining performance levels without manual intervention.
- **Usage:** Especially useful for applications with variable load, ensuring that the deployment scales up during high traffic and scales down during low traffic, thereby managing resource costs effectively.