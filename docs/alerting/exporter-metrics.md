# Metrics collected

Some important metrics are listed below.

| Metrics Name | By | Description |
| --- | --- | --- |
| `configured_gpu_count` | `job_exporter` | number of gpu configured by user |
| `nvidiasmi_utilization_gpu` | `job_exporter` | GPU utilization detectived by nvidiasmi |
| `nvidiasmi_utilization_memory` | `job_exporter` | GPU memory utilization detectiving by nvidiasmi |
| `task_gpu_percent` | `job_exporter` | GPU utilization by specified job container |
| `task_gpu_mem_percent` | `job_exporter` | GPU memory utilization by specified job container |
| `task_cpu_percent` | `job_exporter` | CPU utilization by job detectived by docker stats |
| `task_mem_usage_byte` | `job_exporter` | Memory usage by job detectived by docker stats (byte) |
| `task_mem_limit_byte` | `job_exporter` | Memory limit by job detectived by docker stats (byte) |
| `task_mem_usage_percent` | `job_exporter` | Memory utilization by job detectived by docker stats |
| `task_net_in_byte` | `job_exporter` | Network in traffic by job detectived by docker stats (byte) |
| `task_net_out_byte` | `job_exporter` | Network out traffic by job detectived by docker stats (byte) |
| `task_block_in_byte` | `job_exporter` | Block io in traffic by job detectived by docker stats (byte) |
| `task_block_out_byte` | `job_exporter` | Block io out traffic by job detectived by docker stats (byte) |
| `node_filefd_allocated` | `node_exporter` | Number of file descriptor allocated in node |
| `node_disk_read_time_ms` | `node_exporter` | Node disk read time (ms) |
| `node_disk_write_time_ms` | `node_exporter` | Node disk write time (ms) |
| `node_load1` | `node_exporter` | Node load in past 1 minute |
| `node_filesystem_free` | `node_exporter` | Node filesystem free space (byte) |
| `service_cpu_percent`| `job_exporter` | CPU utilization by pai service detectived by docker stats |
| `service_mem_usage_byte`| `job_exporter` | Memory usage by pai service  detectived by docker stats (byte) |
| `service_mem_limit_byte`| `job_exporter` | Memory limit by pai service detectived by docker stats (byte) |
| `service_mem_usage_percent`| `job_exporter` | Memory utilization by pai service detectived by docker stats |
| `service_net_in_byte`| `job_exporter` | Network in traffic by pai service detectived by docker stats (byte) |
| `service_net_out_byte`| `job_exporter` | Network out traffic by pai service detectived by docker stats (byte) |
| `service_block_in_byte`| `job_exporter` | Block io in traffic by pai service detectived by docker stats (byte) |
| `service_block_out_byte`| `job_exporter` | Block io out traffic by pai service detectived by docker stats (byte) |
| `docker_daemon_count` | `job_exporter` | Used to summary the count of docker daemon, value of this metric is always 1, use "error" label to mark if daemon is healthy or not, admin can use `sum(docker_daemon_count{"error"!="ok"})` to get the count of unhealthy docker daemon in cluster |
