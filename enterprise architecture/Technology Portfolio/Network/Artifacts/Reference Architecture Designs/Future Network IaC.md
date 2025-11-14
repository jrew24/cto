<p><a target="_blank" href="https://app.eraser.io/workspace/nD3Qo1cKL5tOsNeTlU7c" id="edit-in-eraser-github-link"><img alt="Edit in Eraser" src="https://firebasestorage.googleapis.com/v0/b/second-petal-295822.appspot.com/o/images%2Fgithub%2FOpen%20in%20Eraser.svg?alt=media&amp;token=968381c8-a7e7-472a-8ed6-4a6626da5501"></a></p>

# Architecture Diagram
- High-level diagram showing the workflow from local development to production deployment, including key integrations and decision points.
# Workflow Stages
## Local Development
- Network engineer develops Day 0/Day 1/Day 2 configuration as code on local laptop using Ansible.
## Code Repository and Branching
- Code is pushed to Git repository.
- Initial deployment to lab environment.
## Lab Environment
- Code deployed to lab using GitHub and Ansible.
- Initial testing and validation.
## Virtual Test Environment
- Code promoted to test branch; deployed to virtual environment.
- Automated test cases executed.
- If tests fail, code is revised locally and retested.
## Production Preparation
- Successful code is merged into production branch after peer review and approval.
- Change request created in ServiceNow.
- Change window scheduled.
## Production Deployment
- Automation runs: change request creation, code deployment to production, and automated test execution.
- If test cases fail, automated rollback and ticket closure. Teams will investigate what went wrong and add new test cases.
- If successful, change becomes new baseline and ticket is closed.
# Configuration as Code
- Day 0: Initial device provisioning via ZTP and Ansible.
- Day 1: Base configuration deployment.
- Day 2: Ongoing configuration changes and updates.
# Toolchain Integration
- Ansible for configuration management.
- Git for source control and workflow.
- GitHub for CI/CD automation.
- Cisco CML for lab and virtualized testing.
- ServiceNow for change management automation.
# Approval and Rollback Process
- Peer review required before production merge.
- Automated rollback of changes if test cases fail in production.
- Root cause analysis and new test case creation after rollback events.
# Baseline Management
- Successful production deployments update the configuration baseline.
- All changes tracked and auditable via Git and ServiceNow.



<!-- eraser-additional-content -->
## Diagrams
<!-- eraser-additional-files -->
<a href="/enterprise architecture/Technology Portfolio/Network/Artifacts/Reference Architecture Designs/Future Network IaC-Zero Touch Provisioning (ZTP) & IaC Workflow for Cisco Network Devices-1.eraserdiagram" data-element-id="744GERZkRRKgGhq_LRPyK"><img src="/.eraser/nD3Qo1cKL5tOsNeTlU7c___Auxmsx4R82UQEGCqMRLq2WgcK833___---diagram----bb416fdf7826c62860a02bfb38d20d33-Zero-Touch-Provisioning--ZTP----IaC-Workflow-for-Cisco-Network-Devices.png" alt="" data-element-id="744GERZkRRKgGhq_LRPyK" /></a>
<!-- end-eraser-additional-files -->
<!-- end-eraser-additional-content -->
<!--- Eraser file: https://app.eraser.io/workspace/nD3Qo1cKL5tOsNeTlU7c --->