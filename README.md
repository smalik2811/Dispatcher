🚀 Dispatcher
Dispatcher is a distributed system designed to manage asynchronous background tasks across a cluster of workers. Unlike simple task queues, Dispatcher provides a robust gRPC-based orchestration layer that handles worker life-cycles, task persistence, and failure recovery.

🛠 Key Features
- **Distributed Architecture:** Decoupled Scheduler and Worker nodes communicate over gRPC (HTTP/2).
- **Durable Queuing:** Powered by Redis to ensure tasks survive system restarts.
- **Pull-Based Scaling:** Workers pull tasks based on capacity, providing natural backpressure.
- **Fault Tolerance:** Automatic task re-assignment via worker heartbeat monitoring.
- **Observability:** Built-in metrics for throughput, latency, and task success rates.
