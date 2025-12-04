<p><a target="_blank" href="https://app.eraser.io/workspace/9wP5o04XNkopIHCJbkNl" id="edit-in-eraser-github-link"><img alt="Edit in Eraser" src="https://firebasestorage.googleapis.com/v0/b/second-petal-295822.appspot.com/o/images%2Fgithub%2FOpen%20in%20Eraser.svg?alt=media&amp;token=968381c8-a7e7-472a-8ed6-4a6626da5501"></a></p>

# Overview
- Brief description of the system architecture and its primary goal.
- Summary of the multi cloud/hybrid cloud environment and CDN fronting all web traffic.
# Architecture Components
- Content Delivery Network (CDN)
- Public Cloud Providers (GCP, Azure, AWS)
- Private Cloud / Colocation Facilities
- Network Security Layers (mTLS, Network Access Lists)
- Regional and availability zone considerations
# System Diagram Overview
- High-level diagram of end-user traffic flow to CDN.
- Representation of CDN connections to:
    - Public cloud providers across multiple regions.
    - Private colocation facilities.

- Network security boundaries and controls.
# Data Flow Overview
- Flow of web traffic from end users to CDN.
- Flow from CDN to public cloud application endpoints.
- Flow from CDN to private colocation application endpoints.
# Network Security Overview
- High-level use of mTLS between CDN and public clouds.
- Network Access Lists enabled at public cloud perimeter, restricting access to CDN.
- Security boundaries for private cloud connectivity.
# Deployment Environment
- Description of the production environment spanning multi cloud and hybrid cloud infrastructures.
# Operational Considerations
- Notes on regional availability and redundancy.
- Points of contact between CDN, public cloud, and colocation facilities.



<!-- eraser-additional-content -->
## Diagrams
<!-- eraser-additional-files -->
<a href="/enterprise architecture/Technology Portfolio/Network/Artifacts/Reference Architecture Designs/CDN Fronted Security-Multi-Cloud & Hybrid Cloud Web Traffic Architecture-1.eraserdiagram" data-element-id="joGIAcmbnrWflsZjt-HA_"><img src="/.eraser/9wP5o04XNkopIHCJbkNl___Auxmsx4R82UQEGCqMRLq2WgcK833___---diagram----50d4876ebbbbf14bcab6d3298b9aadb6-Multi-Cloud---Hybrid-Cloud-Web-Traffic-Architecture.png" alt="" data-element-id="joGIAcmbnrWflsZjt-HA_" /></a>
<!-- end-eraser-additional-files -->
<!-- end-eraser-additional-content -->
<!--- Eraser file: https://app.eraser.io/workspace/9wP5o04XNkopIHCJbkNl --->