# Pods

A Pod is the smallest and simplest Kubernetes object. A Pod represents a set of running containers on your cluster.

## Characteristics

- Pods typically run a single main container. In advanced scenarios, a Pod can run multiple containers that need to work closely together.

- Pods are ephemeral by nature, they are created and deleted to match the state of your application as it is scaled and managed across the nodes.

## Usage

Pods encapsulate an application’s container (or containers), storage resources, a unique network IP, and options that govern how the container(s) should run. They represent a "logical host" for one or more containers that share the same context.

## Communication

Containers in a Pod share an IP Address and port space, and can find each other via `localhost`. They can also communicate using standard inter-process communications like SystemV semaphores or POSIX shared memory.

## Management

Managed as a unit, Pods are usually managed by higher-level Kubernetes constructs like Deployments or ReplicaSets.