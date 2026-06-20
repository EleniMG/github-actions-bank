# github-actions-bank

This repo is a place to store various GitHub Actions pipelines.

See the [vulnerability-scanners](https://github.com/EleniMG/vulnerability-scanners) for Trivy, npm and pnpm repo and Docker scans.

## Upcoming additions

### Core CI/CD
1. Python CI pipeline — linting, formatting, tests, coverage, caching, matrix builds.

2. Docker build & push — build image → push to GHCR → attach SBOM/attestations.

3. Deploy to GKE — build → push → apply manifests → rollout status.

4. Helm chart deployment — package chart → push to OCI registry → helm upgrade.


### Security and DevSecOps

1. SAST scanning — CodeQL or Semgrep.

2. Dependency review — block PRs with vulnerable dependencies.

3. Secret scanning enforcement — fail builds if secrets are committed.

### Testing and Quality Workflows

1. Matrix testing — Python versions, OS variations, dependency sets.

2. Integration test workflow — spin up services with Docker Compose.

3. Contract testing — run Pact or schema validation.

4. Coverage reporting — upload HTML coverage as artifact + PR comment.

### Dev Experience

1. Automated PR labelling — label PRs based on paths or titles.

2. Autogenerate changelog — semantic‑release or conventional commits.

3. Preview environments — deploy PR branches to ephemeral environments.

4. Slack notifications — build status → Slack channel.


### Infrastructure

1. Terraform plan & apply — plan on PR, apply on main.

2. Pulumi deployment — IaC with policy checks.

3. Kubernetes manifest validation — kubeconform, OPA, Kyverno.

4. SBOM generation — Syft + upload as artifact.


### Packaging and Release

1. Publish Python package to PyPI — build → test → publish.

2. GitHub Releases automation — tag → changelog → release assets.

3. Version bump automation — semantic versioning.


AI & Automation 

1. Generate documentation with LLMs — auto‑summaries or PR descriptions.

2. Automated code review suggestions — annotate PRs with suggestions.

3. Test data generation — generate fixtures or mocks.