# Optimizing inactive cloud workloads in CrownLabs
This repo is intended to be a quick documentation and report about the work done to implement an inactive resource optimization policy in [CrownLabs](https://github.com/netgroup-polito/CrownLabs).

## Requirements
- [ ] Inactive detection policy (initially based on Tenant last login, could be extended to instance metrics such as workload or ingress/proxy access)
- [ ] Tenant notification when an inactive instance is detected (email)
- [ ] Instance pause/deletion after max inactive time
- [ ] (opt.) Adjust pod resource limits based on the actual consumptions 
- [ ] (opt.) Live migration for resource consolidation among worker nodes


# REPORTS ACHIEVEMENTS
- `31/03 - 06/04`: First architecture alternatives
- `07/04 - 13/04`: Prometheus-stack installed; Achieved good capability to interact with PromQL, setting custom Alert rules;
- `14/04 - 20/04`: Definition and tests of local development environment
- `21/04 - 27/04`: Local deployment enviroment testing
- `28/04 - 04/05`: Developed a demo implementation of the `InstanceInactiveController`.
- `05/05 - 11/05`: Refined logic for the termination mechanism
- `12/05 - 18/05`: Implementation of Prometheus checks for `InstanceInactiveController`, implementation of mail notification service
- `19/05 - 25/05`: Implementation tests
- `26/05 - 01/06`: Implementation tests
- `26/05 - 01/06`: Implementation of new Grafana Dashboard for Crownlabs resource usage and consumption
- `02/06 - 08/06`: Implementation bastion SSH checks
- `09/06 - 15/06`: Fixes after Review comments, Refined Grafana Dashboard
- `16/06 - 22/06`: Fixes after Review comments, Refined Grafana Dashboard
