# Oleksandr Zaiats

**Senior Platform / DevOps Engineer · AWS · Kubernetes · Terraform · SRE**

I design, build and operate cloud platforms that help engineering teams ship software independently, with clear boundaries around access, reliability and cost. My work connects platform architecture with hands-on implementation and production operations.

Based in Germany, open to international remote opportunities and B2B collaborations. English is my technical working language.

[LinkedIn](https://www.linkedin.com/in/alexandrzayats/) · [EnvPlane](https://envplane.dev/) · [Email](mailto:alex@zaiats.de)

## Platform engineering and reliability

- **Cloud foundations:** AWS architecture, Kubernetes/EKS, networking, IAM and Linux.
- **Developer platforms:** reusable Terraform/Terragrunt modules, self-service environments and automated provisioning and teardown.
- **Software delivery:** GitHub Actions, GitLab CI, GitOps, Helm and Ansible.
- **Production reliability:** Prometheus, Grafana, ELK/EFK, SLO/SLA responsibility, on-call, incident response and root-cause analysis.

My professional background includes building and operating a greenfield AWS/Kubernetes platform at Betario, creating production-like developer environments, and improving deployment workflows and observability. I value platforms that teams can understand, operate and maintain without depending on one person.

## Selected public projects

These repositories show platform tooling, reference implementations and reusable infrastructure components. See each repository for its architecture, setup and project-specific guidance.

| Project | Focus |
| --- | --- |
| [Kubernetes Admin Gateway](https://github.com/Alexandr-Zayats/multi-environment-admin-gateway-platform) | Go control plane and Next.js frontend for on-demand administrative consoles, with OIDC, RBAC and Kubernetes integration. |
| [kctx](https://github.com/Alexandr-Zayats/kctx) | Go tooling for Kubernetes context switching across AWS, GCP and DigitalOcean, including AWS SSO support. |
| [Terraform modules](https://github.com/Alexandr-Zayats/devops-terraform) | Reusable infrastructure modules for AWS, Google Cloud and Kubernetes. |
| [Terragrunt stacks](https://github.com/Alexandr-Zayats/devops-terragrunt) | Composable stacks and units for multi-environment cloud infrastructure. |
| [FluxCD platform configuration](https://github.com/Alexandr-Zayats/devops-fluxcd) | GitOps-managed Kubernetes manifests and platform services. |
| [Helm platform charts](https://github.com/Alexandr-Zayats/helm-platform-charts) | Reusable charts for namespace governance, maintenance routing and ECK observability. |
| [GitLab CI building blocks](https://github.com/Alexandr-Zayats/devops-gitlab-ci) | Reusable build, test, release and deployment templates. |

## Building EnvPlane

[EnvPlane](https://envplane.dev/) is my independent environment-orchestration project, currently in private preview. It focuses on the lifecycle of Kubernetes environments: from a source-control event through deployment, operational visibility and teardown.

The architecture separates central coordination from execution near the target cluster, with Helm and Flux CD delivery paths. Current work includes scoped access, auditability and cost visibility.

[Explore the EnvPlane repositories](https://github.com/EnvPlane)

## Exploring AI infrastructure

Alongside my established platform work, I am developing practical experience with local AI inference and agent workflows. My recent work includes a local MLX inference server with an OpenAI-compatible API, structured outputs, evaluations and human approval workflows.

The engineering question I focus on is how to give agents useful capabilities while keeping permissions, execution and verification under explicit control.

## Engineering principles

- Keep repeatable operational knowledge in code, pipelines and documented workflows.
- Use least privilege, short-lived identity and auditable access.
- Design for recovery with observable systems and reversible changes.
- Remove developer toil without hiding essential system behavior.

## Connect

Interested in senior platform engineering, developer self-service, production reliability or AI infrastructure? Reach out on [LinkedIn](https://www.linkedin.com/in/alexandrzayats/) or at [alex@zaiats.de](mailto:alex@zaiats.de).

For EnvPlane product and early-access inquiries: [hello@envplane.dev](mailto:hello@envplane.dev).
