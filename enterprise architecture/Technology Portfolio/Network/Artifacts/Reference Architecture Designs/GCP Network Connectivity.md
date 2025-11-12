<p><a target="_blank" href="https://app.eraser.io/workspace/gcZavrS28ONsMgSO5Ohx" id="edit-in-eraser-github-link"><img alt="Edit in Eraser" src="https://firebasestorage.googleapis.com/v0/b/second-petal-295822.appspot.com/o/images%2Fgithub%2FOpen%20in%20Eraser.svg?alt=media&amp;token=968381c8-a7e7-472a-8ed6-4a6626da5501"></a></p>

### **Summary**
**Overview**

In this network topology, Interconnect (or HA-VPN) from on-premises (or other clouds) terminates directly into the Shared VPC of each workload environment.

This pattern provides hybrid connectivity to:

1. IaaS resources in the workload Shared VPC Networks
2. Google APIS and services (e.g. storage.googleapis.com, *. run.app etc) in the workload projects
3. Google Cloud managed services tat use [﻿Private Services Access](https://docs.cloud.google.com/vpc/docs/private-services-access)  
**Use this pattern when...**
4. You have many workload VPC Networks that can share a common Interconnect to on-premises or other clouds. In this example, we show only two Shared VPC networks. The same Interconnect can be used by multiple Shared VPC networks. Each shared VPC attaches to the same interconnect via separate VLAN attachments.
5. You may not require network connectivity between all workload shared VPC Networks. If connectivity is required between the Shared VPC networks, you can consider the options highlighted in [﻿Connecting Multiple VPC Networks](https://docs.cloud.google.com/network-connectivity/docs/interconnect/how-to/enabling-multiple-networks-access-same-attachment)  
6. You require network connectivity from on-premises to managed services that use Private Services Access (ie VPC Peering) to the workload Shared VPC networks. This pattern allows access to any managed services from on-premises and all workload Shared VPC Networks.
**Scaling out (larger Number of Shared VPC networks)**
An Interconnect supports a maximum of 16 VLAN attachments. This means we can have a maximum of 16 Shared VPC Networks in this pattern. You can scale out by adding more Interconnects to accomodate additional Shared VPC networks.






<!-- eraser-additional-content -->
## Diagrams
<!-- eraser-additional-files -->
<a href="/enterprise architecture/Technology Portfolio/Network/Artifacts/Reference Architecture Designs/GCP Network Connectivity-GCP Hybrid Connectivity to Multiple VPC or Shared VPC-1.eraserdiagram" data-element-id="htIhf8TpOPvKEenuv7X0A"><img src="/.eraser/gcZavrS28ONsMgSO5Ohx___Auxmsx4R82UQEGCqMRLq2WgcK833___---diagram----bddd2a8202844722533d025efcf9c968-GCP-Hybrid-Connectivity-to-Multiple-VPC-or-Shared-VPC.png" alt="" data-element-id="htIhf8TpOPvKEenuv7X0A" /></a>
<!-- end-eraser-additional-files -->
<!-- end-eraser-additional-content -->
<!--- Eraser file: https://app.eraser.io/workspace/gcZavrS28ONsMgSO5Ohx --->