# Oleksandr Zaiats

**Senior Platform / DevOps Engineer · AWS · Kubernetes · Terraform · SRE**

I design, build and operate cloud platforms that help engineering teams ship software independently, with clear boundaries around access, reliability and cost. My work connects platform architecture with hands-on implementation and production operations.

Systems and infrastructure engineering since **2009**, AWS since **2013**, and Kubernetes since **2017**.

Based in Germany and available full-time for permanent employment or B2B engagements with international remote teams. Available to start within 1-2 days. English is my technical working language; German: A2.

[LinkedIn](https://www.linkedin.com/in/alexandrzayats/) · [EnvPlane](https://envplane.dev/) · [Email](mailto:alex@zaiats.de)

## Platform engineering and reliability

- **Cloud foundations:** AWS architecture, Kubernetes/EKS, networking, IAM and Linux.
- **Developer platforms:** reusable Terraform/Terragrunt modules, self-service environments and automated provisioning and teardown.
- **Software delivery:** GitHub Actions, GitLab CI, GitOps, Helm and Ansible.
- **Production reliability:** Prometheus, VictoriaMetrics, Grafana, Elasticsearch/Kibana, internal SLOs, PagerDuty on-call, incident response and root-cause analysis.

At **Betario**, I independently designed and implemented Kubernetes infrastructure and GitLab CI pipelines for **3 teams of approximately 30 specialists**. The platform comprised **6 clusters across 4 AWS accounts**, with about **25 application microservices per environment**. I worked with developers to define microservice boundaries and supported adoption through presentations, Confluence documentation and onboarding.

- Reduced full feature-environment provisioning from **30-40 to 5-7 minutes**, with capacity to deploy up to **20 separate feature environments per day**. Each had its own namespace, S3 bucket and database; closing the merge request triggered full cleanup.
- Built VictoriaMetrics, Grafana and Elasticsearch/Kibana observability, severity-based escalation and weekly PagerDuty on-call rotations. The internal availability objective allowed up to **5 minutes of total downtime per week**.
- Reduced the **longest observed investigation and resolution time** from up to **4 hours to 40 minutes**. This concerns issue resolution, including partially degraded services, not mean MTTR or full-outage duration.
- Production operated for **over 360 days without an incident causing application unavailability**. Actual concurrent users grew from **2,000 to 20,000**. The average daily failed API/HTTP request rate fell from **3.5% to about 1.5%**, sustained for the rest of my tenure.

At **HRS**, I proposed and implemented similar self-service workflows in an engineering organisation of more than 100 developers across approximately 10 teams.

At **Suntech Innovation**, I automated Jenkins provisioning with Terraform and independently designed and implemented a replacement for Datadog Enterprise using self-hosted Elasticsearch/Kibana. The phased migration saved approximately **$10,000 net per month**, including replacement infrastructure costs. Existing self-service practices predated my arrival.

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

[EnvPlane](https://envplane.dev/) is my independent environment-orchestration project, developed in my spare time alongside professional commitments. It is in internal beta, with no external users yet. It focuses on the lifecycle of Kubernetes environments: from a source-control event through deployment, operational visibility and teardown.

The architecture separates central coordination from execution near the target cluster, with Helm and Flux CD delivery paths. Current work includes scoped access, auditability and cost visibility.

[Explore the EnvPlane repositories](https://github.com/EnvPlane)

## Exploring AI infrastructure

I am developing and internally testing **13 AI agents** in EnvPlane for configuration analysis, deployment troubleshooting and cost estimation. Inputs include YAML/Helm configuration, UI forms, API errors and Kubernetes state.

Agent configuration supports recommendations, human-approved changes or automatic changes through EnvPlane, including removal of resources managed by the platform. Human approval is configurable, not mandatory for every action.

Cost estimates combine project-configured costs, EnvPlane pricing and AI token usage costs. Additional cloud resources are estimated from information available to the agent; this is not a claim of live cloud billing integration. External user rollout is planned.

I also work with a local MLX inference server and an OpenAI-compatible API.

The engineering question I focus on is how to give agents useful capabilities while keeping permissions, execution and verification under explicit control.

## Engineering principles

- Keep repeatable operational knowledge in code, pipelines and documented workflows.
- Use least privilege, short-lived identity and auditable access.
- Design for recovery with observable systems and reversible changes.
- Remove developer toil without hiding essential system behavior.

## Connect

Interested in senior platform engineering, developer self-service, production reliability or AI infrastructure? Reach out on [LinkedIn](https://www.linkedin.com/in/alexandrzayats/) or at [alex@zaiats.de](mailto:alex@zaiats.de).

For EnvPlane product and early-access inquiries: [hello@envplane.dev](mailto:hello@envplane.dev).
