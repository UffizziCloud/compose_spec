# The Uffizzi Compose Specification  

This document specifies the Uffizzi Compose file format used to define and preview multi-container applications using Uffizzi. A Uffizzi Compose file is a structured YAML format, similar to Docker Compose. Uffizzi Compose is based on Compose version 3.9, but it also includes additional parameters relevant to Uffizzi Continuous Previews. This document describes the required and optional parameters of Uffizzi Compose.

### Uffizzi Compose file  
The Uffizzi Compose file is a YAML file defining services (REQUIRED) and configs.

### Services (required)

As with Docker Compose, a Service is an abstract definition of a computing resource within an application which can be scaled/replaced independently from other components. Services are backed by a set of containers when deployed on Uffizzi.  The following table outlines the support status of the Services sub-level elements:   


| Compose Element                        | Uffizzi Compose Support Status |
| -------------------------------------- | ------------------------------ |
| **Services (Top-level)**               | Supported                      |
| deploy                                 | Supported                      |
| blkio_config                           | Unsupported (not planned)      |
| device_read_bps, device_write_bps      | Unsupported (not planned)      |
| device_read_iops, device_write_iops    | Unsupported (not planned)      |
| weight                                 | Unsupported (not planned)      |
| weight_device                          | Unsupported (not planned)      |
| cpu_count                              | Unsupported (not planned)      |
| cpu_percent                            | Unsupported (not planned)      |
| cpu_shares                             | Unsupported (not planned)      |
| cpu_period                             | Unsupported (not planned)      |
| cpu_quota                              | Unsupported (not planned)      |
| cpu_rt_runtime                         | Unsupported (not planned)      |
| cpu_rt_period                          | Unsupported (not planned)      |
| cpus                                   | Unsupported (not planned)      |
| cpuset                                 | Unsupported (not planned)      |
| build                                  | Supported                      |
| cap_add                                | Unsupported (not planned)      |
| cap_drop                               | Unsupported (not planned)      |
| cgroup_parent                          | Unsupported (not planned)      |
| command                                | Unsupported (planned)          |
| configs                                | Supported                      |
| container_name                         | Unsupported (not planned)      |
| credential_spec                        | Unsupported (not planned)      |
| depends_on                             | Unsupported (planned)          |
| device_cgroup_rules                    | Unsupported (not planned)      |
| devices                                | Unsupported (not planned)      |
| dns                                    | Unsupported (not planned)      |
| dns_opt                                | Unsupported (not planned)      |
| dns_search                             | Unsupported (not planned)      |


### Services (required)

As with Docker Compose, a Service is an abstract definition of a computing resource within an application which can be scaled/replaced independently from other components. Services are backed by a set of containers when deployed on Uffizzi.  
