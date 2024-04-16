# Batch Execution

Kubernetes supports batch execution via [[Jobs]] and [[CronJobs]], allowing for the running of one-off or periodic tasks that complete a specific job rather than hosting continuous services.

## Functionality

- **[[Jobs]]:** Manage a workload that runs to completion, for instance processing a batch of data or performing a database migration.

- **[[CronJobs]]:** Schedule Jobs to run periodically at fixed times/dates, much like the Unix cron tool.

## **Usage:**

Useful for maintenance tasks, backups, batch processing, and other tasks that need to run periodically or just once.

## **Benefits:**

Automates repetitive tasks, ensuring they are executed reliably and without manual intervention, which helps in managing routine tasks efficiently and predictably.