# Moving Airflow Sensors to Async Execution

A case study on migrating 3,500 Airflow sensors (~2,500 concurrent) from Worker slots to the
Triggerer's asyncio event loop — including a heartbeat-blocking `bulk_fetch`
JOIN, DB load reduction, isolated-cluster verification, a DAG-hash based
progressive rollout, and an upstream patch to Apache Airflow
([#68792](https://github.com/apache/airflow/pull/68792)).

📄 **[Read the case study →](https://jh0917.github.io/airflow-async-sensor/)**

Apache Airflow 2.6.2 · Python asyncio · LocalExecutor · Kubernetes
