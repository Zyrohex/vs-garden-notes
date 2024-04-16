# Replication Controller

A Replication Controller ensures that a specified number of [[Pod Replicas]] are running at any given time. It is one of the earlier Kubernetes controllers, **now largely superseded by [[Deployments]] which offer more features and flexibility.**

## Functionality

- It monitors the number of pods in its charge, creating or killing pods as needed to reach the desired count.

- It handles pod failures by replacing the failed pods to ensure the application continues to run as expected.

## Configuration

A Replication Controller is defined with a Pod template, which it uses to create actual pods. The configuration includes the desired number of replicas and the selectors to identify the pods it manages.

## Benefits

Guarantees the availability of a specific number of identical pods, which is crucial for fault tolerance and high availability of services.

## Usage

While still usable, it is recommended to use Deployments for new applications, as Deployments manage the lifecycle of pods and their updates more effectively and provide features like rollbacks and fine-grained updates.