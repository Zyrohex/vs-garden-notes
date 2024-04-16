# Persistent Volume Claim

A Persistent Volume Claim (PVC) is a request for storage by a user. It is similar to a Pod in that Pods consume node resources, while PVCs consume [[Persistent Volume Resources]].

## Characteristics

- PVCs specify size, and access modes (such as read-write or read-only).
- A PVC, once created, is automatically bound to an available PV in the cluster that meets its requirements, if available.
- If no suitable PV exists, the PVC remains unbound indefinitely until a suitable PV is created.

## Usage

PVCs allow a user to abstract the details of the storage being requested. Developers only need to be aware of the claim to storage, without needing to be concerned about the actual physical storage specifics.

## Dynamic Provisioning

When a PVC is created, a corresponding PV can be dynamically provisioned through a StorageClass, depending on the configuration. This decouples the task of configuring underlying storage from the usage of storage in Pods.