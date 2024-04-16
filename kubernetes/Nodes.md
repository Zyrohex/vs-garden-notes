# Nodes

A Node is a worker machine in Kubernetes, which may be either a virtual or a physical machine, depending on the cluster.

## Characteristics

- Each Node is managed by the master components and contains the services necessary to run Pods, managed by the Kubernetes runtime environment (Docker, CRI-O, etc.).

- Nodes include the Kubelet, which is the primary "node agent" that acts on commands from the Master to manage the Pods and their containers.

## Responsibilities

Nodes handle the networking between Kubernetes control plane and pods, manage assigned pods, monitor resource usage, and report back to the master. They also handle the orchestration and execution of application containers based on workload schedules.

## Health Monitoring

Nodes are monitored for their health status by the master components. If a node fails, the Pods running on that node are automatically moved to other nodes in the cluster.