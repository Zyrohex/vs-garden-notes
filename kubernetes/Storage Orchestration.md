# Storage Orchestration

Kubernetes allows for the automatic management of storage resources through its storage orchestration capabilities.

## Functionality

Kubernetes enables the dynamic provisioning of storage resources through [[Persistent Volumes]] (PV) and [[Persistent Volume Claims]] (PVC). It supports automatic mounting of storage systems such as local storage, public cloud providers, and more.

## Benefits

This feature allows developers to request storage resources without needing to know the details of the underlying storage infrastructure, thereby simplifying the process of configuring and using storage with applications.