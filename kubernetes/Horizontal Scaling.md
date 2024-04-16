# Horizontal Scaling

Horizontal scaling in Kubernetes involves increasing or decreasing the number of [[Pod Replicas]] of an application to adjust to the load without changing any of the Pod’s resources.

## Mechanism

This is typically managed by the [[Horizontal Pod Autoscaler (HPA)]], which automatically scales the number of Pods in a [[Replication Controller]], deployment, replica set, or stateful set based on observed CPU utilization or other select metrics provided by custom metrics APIs.

## Usage

Horizontal scaling is crucial for applications with varying loads, ensuring performance remains consistent as demands increase.

## Benefits

Enhances the application's availability and performance by dynamically allocating resources based on real-time processing demands, thus improving resource efficiency.