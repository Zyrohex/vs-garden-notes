# Persistent Volumes

A Persistent Volume (PV) is a [[Persistent Volume Resources]] in a [[Cluster]] that has been provisioned by an administrator or dynamically provisioned using [[Storage Classes]]. It is a piece of storage in the cluster that has been provisioned independently of the usage of individual [[Pods]].

## Characteristics

- PVs are volume plugins like Volumes but have a lifecycle independent of any individual Pod that uses the PV.
- A PV is a cluster-wide resource, similar to a node that is a cluster resource.
- PVs can have various underlying storage backends, such as NFS, iSCSI, or cloud-specific storage APIs.

## Usage

PVs are intended for use with applications that require persistent storage. The storage itself is provided by an external resource, the configuration of which is managed at the Kubernetes admin level, not by individual developers.