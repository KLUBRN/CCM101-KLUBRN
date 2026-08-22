# Cloud Provider Comparison

## Equivalent Infrastructure Services

| Infrastructure Component | AWS | Microsoft Azure | Google Cloud Platform |
|---|---|---|---|
| Compute | EC2 (Elastic Compute Cloud) | Virtual Machines | Compute Engine |
| Storage | S3 (Simple Storage Service) | Blob Storage | Cloud Storage |
| Networking | VPC (Virtual Private Cloud) | Virtual Network (VNet) | VPC (Virtual Private Cloud) |
| Identity and Access Management (IAM) | AWS IAM | Microsoft Entra ID (formerly Azure AD) | Cloud IAM |

## Guide Questions

**1. Which cloud provider offers the broadest range of services? Explain your answer.**
AWS has the widest service catalog by a clear margin, with well over 200 offerings that go far beyond the basics — things like ground station access for satellites and experimental quantum computing tools. Being the earliest major player in the space gave it a head start on building out that breadth.

**2. Which cloud platform would you recommend for an organization that primarily uses Microsoft products?**
Azure fits best for a Microsoft-centric organization, since it plugs directly into tools like Active Directory, 365, and .NET without extra work. Because Entra ID handles identity across the whole Microsoft stack, staff can log into everything with one account instead of juggling separate systems.

**3. Which platform is widely recognized for Artificial Intelligence (AI), Machine Learning (ML), and Kubernetes services?**
Google Cloud stands out here — Kubernetes itself originated at Google, and its managed version (GKE) is generally seen as the most polished implementation available. On the AI/ML side, Vertex AI and Google's own TPU chips give it an edge for training and running models.

**4. What similarities did you observe among the three cloud providers?**
Strip away the branding and all three are built around the same four building blocks — compute, storage, networking, and identity management. They also share a similar business model: pay only for what you use, data centers spread across the globe, and roughly comparable core capabilities — so choosing between them usually comes down to ecosystem fit and cost rather than one being fundamentally more capable.
