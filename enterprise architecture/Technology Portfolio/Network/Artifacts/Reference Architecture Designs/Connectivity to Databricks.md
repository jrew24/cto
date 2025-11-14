<p><a target="_blank" href="https://app.eraser.io/workspace/wXAapOwxzyTgw5FlnGCF" id="edit-in-eraser-github-link"><img alt="Edit in Eraser" src="https://firebasestorage.googleapis.com/v0/b/second-petal-295822.appspot.com/o/images%2Fgithub%2FOpen%20in%20Eraser.svg?alt=media&amp;token=968381c8-a7e7-472a-8ed6-4a6626da5501"></a></p>

# Reference Architectures for Connecting to Databricks SaaS on AWS
## Overview
This document outlines three high-level architectures for establishing secure connectivity to a Databricks SaaS instance hosted in AWS. Each scenario addresses connectivity from different network origins, emphasizing security, performance, scalability, and operational complexity.

---

## Scenario 1: Non-AWS Source via Colocation Facility
**Description:**
A non-AWS environment connects through a colocation facility (e.g., Equinix) to a trusted AWS VPC, which then accesses Databricks via AWS PrivateLink.

**Architecture Diagram:**
_Insert diagram here._

**Key Components:**

- Non-AWS source (e.g., GCP, Azure, private datacenter)
- Colocation facility (Equinix)
- Trusted AWS VPC
- AWS PrivateLink
- Databricks VPC
**Security Considerations:**

- Controlled ingress/egress at colocation facility
- VPC-level trust boundaries
- Encrypted data in transit
**Performance Optimization:**

- Low-latency private connectivity via colocation
- Bandwidth planning for cross-network traffic
**Scalability:**

- Expandable VPC and PrivateLink endpoints
- Accommodates additional non-AWS sources
**Operational Complexity:**

- Multi-provider network management
- Coordination across colocation and cloud environments
---

## Scenario 2: Trusted AWS VPC to Databricks via PrivateLink
**Description:**
A trusted AWS VPC connects directly to the Databricks VPC over AWS PrivateLink.

**Architecture Diagram:**
_Insert diagram here._

**Key Components:**

- Trusted AWS VPC
- AWS PrivateLink
- Databricks VPC
**Security Considerations:**

- Restricted VPC access policies
- No internet exposure for Databricks endpoints
**Performance Optimization:**

- Intra-cloud low-latency connectivity
- Scalable PrivateLink endpoints
**Scalability:**

- Easily deploy additional VPCs with PrivateLink access
**Operational Complexity:**

- Simplified management within AWS ecosystem
---

## Scenario 3: Untrusted AWS VPC to Databricks via PrivateLink
**Description:**
An untrusted AWS VPC connects directly to the Databricks VPC using AWS PrivateLink.

**Architecture Diagram:**
_Insert diagram here._

**Key Components:**

- Untrusted AWS VPC
- AWS PrivateLink
- Databricks VPC
**Security Considerations:**

- Enhanced VPC endpoint controls
- Monitoring and auditing of access patterns
**Performance Optimization:**

- Direct, private connectivity
- Potential need for network segmentation
**Scalability:**

- Supports multiple untrusted VPCs with controlled access
**Operational Complexity:**

- Requires strict security controls and monitoring
---

## Additional Notes
- Integration with other services (e.g., Snowflake, S3) may require additional networking considerations.
- Diagrams should illustrate the network boundaries and flow of data per scenario.



<!-- eraser-additional-content -->
## Diagrams
<!-- eraser-additional-files -->
<a href="/enterprise architecture/Technology Portfolio/Network/Artifacts/Reference Architecture Designs/Connectivity to Databricks-Reference Architectures for Connecting to Databricks SaaS on AWS-1.eraserdiagram" data-element-id="uNGdRBf7m69XVjNIt6Rgm"><img src="/.eraser/wXAapOwxzyTgw5FlnGCF___Auxmsx4R82UQEGCqMRLq2WgcK833___---diagram----25d5b853848120dc43f35ba197c85e59-Reference-Architectures-for-Connecting-to-Databricks-SaaS-on-AWS.png" alt="" data-element-id="uNGdRBf7m69XVjNIt6Rgm" /></a>
<!-- end-eraser-additional-files -->
<!-- end-eraser-additional-content -->
<!--- Eraser file: https://app.eraser.io/workspace/wXAapOwxzyTgw5FlnGCF --->