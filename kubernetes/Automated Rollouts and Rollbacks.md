# Automated Rollouts and Rollbacks

Automated rollouts and rollbacks are features that allow Kubernetes to change the actual state of a [[Deployed Application]] to the desired state at a controlled rate.

## Functionality

- **Rollouts** Update to new versions of application containers without downtime, ensuring that any new changes are made incrementally to replace old Pods with new ones.

- **Rollbacks** Automatically revert to a previous version of application deployment if the current rollout fails, based on defined health checks and metrics.

## Usage

These features are managed through Kubernetes [[Deployments]], which can be configured to specify the desired number of replicas, allowing updates and rollbacks to be handled without manual intervention.

## Benefits

Provides high availability by ensuring that the application is not down during updates, and safe deployment practices by automatically reverting to a known good state in case of failure.