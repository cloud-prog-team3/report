# Optimizing inactive cloud workloads in CrownLabs
This repo is intended to be a quick documentation and report about the work done to implement an inactive resource optimization policy in [CrownLabs](https://github.com/netgroup-polito/CrownLabs).

## Requirements
- [ ] Inactive detection policy (initially based on Tenant last login, could be extended to instance metrics such as workload or ingress/proxy access)
- [ ] Tenant notification when an inactive instance is detected (email)
- [ ] Instance pause/deletion after max inactive time
- [ ] (opt.) Adjust pod resource limits based on the actual consumptions 
- [ ] (opt.) Live migration for resource consolidation among worker nodes
