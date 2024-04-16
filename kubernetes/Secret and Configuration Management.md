# Secret and Configuration Management

Kubernetes provides built-in support for managing sensitive information ([[Secrets]]) and application configurations ([[ConfigMaps]]).

## Components

- **[[Secrets]]:** Used to store and manage sensitive information such as passwords, OAuth tokens, and ssh keys. They can be mounted as data volumes or exposed as [[Environment Variables]] to be used by Pods in a cluster.

- **[[ConfigMaps]]:** Used to store non-sensitive configuration data in key-value pairs. This can also be mounted as volumes or exposed as environment variables.

## Usage

Both Secrets and ConfigMaps are decoupled from container images, reducing the risk of sensitive data exposure and allowing applications to be easily portable across environments with different configurations.

## Benefits

- Enhances security by separating sensitive information from the application code and improves flexibility in application deployment and configuration.