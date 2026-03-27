# DevOps / Build & Release Engineer Interview Preparation

## 1. Build & Release Engineer

### What is the role of a Build & Release Engineer?
A Build & Release Engineer is responsible for automating the software build, integration, and deployment processes. They ensure consistent and reliable releases by creating CI/CD pipelines, managing artifacts, handling versioning, and coordinating deployments across environments.

---

### What CI/CD tools have you worked with?
Common tools include:
- Jenkins
- Azure DevOps
- GitHub Actions
- GitLab CI/CD
- Bamboo  
Also used Docker, Kubernetes, Terraform for deployment automation.

---

### How do you design a CI/CD pipeline from scratch?
1. Integrate source control (Git)
2. Define stages: Build → Test → Package → Deploy
3. Add automated unit/integration tests
4. Configure artifact storage
5. Set up deployment strategies (blue-green/canary)
6. Add monitoring and rollback mechanisms

---

### How do you automate build, packaging, and deployment?
- Use pipeline tools (Azure DevOps/Jenkins)
- Use scripts (Shell/PowerShell)
- Use Docker for packaging
- Use Terraform/ARM templates for infrastructure provisioning

---

### How do you handle build failures?
- Analyze logs
- Identify root cause
- Fix code/configuration issues
- Re-run pipeline
- Add alerts and fail-fast mechanisms

---

### How do you optimize build time?
- Parallel execution
- Cache dependencies
- Incremental builds
- Optimize tests
- Use lightweight containers

---

### How do you manage artifacts?
Artifacts are stored in repositories like:
- Nexus
- Artifactory
- Azure Artifacts  
Use versioning and retention policies.

---

### How do you define versioning strategies?
Use Semantic Versioning:
MAJOR.MINOR.PATCH  
Automate version tagging using Git.

---

### How do you manage secrets in pipelines?
Use:
- Azure Key Vault
- HashiCorp Vault  
Avoid storing secrets in code.

---

### What is release management?
It involves planning, scheduling, and controlling software releases, including approvals, rollback strategies, and stakeholder communication.

---

## 2. CI/CD Scenarios

### What are stages in a CI/CD pipeline?
- Source
- Build
- Test
- Package
- Deploy
- Monitor

---

### If pipeline succeeds but nothing deploys?
Possible reasons:
- Deployment stage skipped
- Misconfigured triggers
- Missing approvals
- Wrong environment configuration

---

### Why pipeline triggers twice?
- Multiple triggers (PR + commit)
- Duplicate webhook configuration
- Multiple pipeline definitions

---

### How to deploy different configs per environment?
Use:
- Environment variables
- Parameterized pipelines
- Config files (dev.tfvars, prod.tfvars)

---

### How to improve slow pipeline?
- Parallel jobs
- Optimize scripts
- Reduce dependencies
- Enable caching

---

### How to pass variables between stages?
- Pipeline variables
- Output variables
- Artifacts

---

## 3. Azure DevOps

### What is a Service Connection?
A secure connection between Azure DevOps and external services like Azure, AWS, or Docker registries.

---

### Can Azure DevOps work without Azure?
Yes, it supports multi-cloud and on-premise environments.

---

### Branching strategy?
- GitFlow
- Trunk-based development

---

### Direct commits to main?
Not recommended. Use pull requests with approvals.

---

## 4. Kubernetes

### What is a Deployment?
Manages stateless applications and ensures desired replicas.

---

### What is a StatefulSet?
Used for stateful apps with persistent storage and stable identity.

---

### Difference between Deployment and StatefulSet?
- Deployment → Stateless
- StatefulSet → Stateful

---

### How does app connect to DB in Kubernetes?
Using Kubernetes Service (DNS-based communication).

---

### What is a port?
A communication endpoint for containers.

---

## 5. Terraform

### What is a Terraform module?
Reusable block of infrastructure code.

---

### What is a provisioner?
Executes scripts after resource creation.

---

### Types of provisioners?
- local-exec
- remote-exec
- file

---

### What is variables.tf?
Defines input variables.

---

### Managing environments in Terraform?
- Workspaces
- tfvars files

---

## 6. Linux & Shell

### Check disk usage
df -h  
du -sh

---

### Difference between $* and $@
$* → all arguments as one string  
$@ → arguments as separate strings

---

### Replace text in file
sed -i 's/old/new/g' file.txt

---

## 7. Monitoring

### Why alert at 80% disk usage?
Prevents outages before disk is full.

---

## 8. Code Quality

### Tools used
- SonarQube
- Snyk
- Checkmarx

---

### What is quality gate?
A set of conditions that must pass before deployment.

---

## 9. Git & Branching

### Multiple developers on same branch?
- Pull latest changes
- Resolve conflicts
- Use PRs

---

### Deployment branches
- Dev → develop
- Prod → main/master

---

## 10. YAML Pipelines

### Single YAML for multiple environments?
Yes, using parameters and variables.

---

### Dev stage fails?
Fix issue before promoting to QA/Prod.

---

## 11. Terraform Advanced

### What files are used?
- main.tf
- variables.tf
- outputs.tf
- backend.tf

---

### Passing variables
- CLI (-var)
- tfvars files
- environment variables

---

## 12. Agile

### Methodology used?
Agile (Scrum/Kanban)

---

### Agile implementation?
- Sprint planning
- Daily standups
- Retrospectives

---

## 13. Azure Boards

### Add fields to User Story?
Customize process template in Azure DevOps.

---

## 14. Azure DevOps Features

### Library, Artifacts, Environments?
- Library → variables/secrets
- Artifacts → package storage
- Environments → deployment targets

---

## 15. Secure Files

### How to store?
Use Azure DevOps secure files and reference in pipelines.

---

## 16. Additional Concepts

### What is CI/CD?
Continuous Integration and Continuous Deployment.

---

### Pipeline types in Azure DevOps?
- Build pipeline
- Release pipeline

---

### What is Application Gateway?
Layer 7 load balancer with routing features.

---

### Load balancer types in Azure?
- Public
- Internal

---

### What is Terragrunt?
Wrapper for Terraform to manage environments.

---

### What is null resource?
A placeholder resource used to execute scripts.

---

### What is AKS upgrade?
Upgrading Kubernetes cluster version.

---

### Traffic splitting (40/60)?
Use Azure Traffic Manager with weighted routing.

---

## 17. Final Interview Question

### Why should we hire you?
I bring strong expertise in CI/CD, cloud platforms, infrastructure as code, and automation. I focus on improving deployment reliability, reducing failures, and optimizing delivery pipelines.
