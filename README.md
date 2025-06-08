# Google Cloud Platform Systems Analysis and Design (SAD)

This repository contains case studies, each scoped to their own branch, that demonstrate systems analysis and design approaches leveraging Google Cloud Platform services across diverse industries and use cases. The repository is industry-agnostic, focusing on the strategic alignment of GCP services with specific business and technical requirements.

Each case study applies a comprehensive problem-solving methodology that views system design as 'a search or problem-solving process that uses means to achieve desired ends' ([Strohmann et al., 2023](https://lutpub.lut.fi/bitstream/handle/10024/166324/strohmann_et_al_design_principles_publishers_version.pdf?sequence=3&isAllowed=y)). This holistic approach integrates multiple types of knowledge from understanding the problem domain to developing practical solutions, creating a framework that addresses the complex, interconnected challenges found in modern cloud architectures.

The methodology's strength lies in its proven versatility across diverse technical domains, making it particularly effective for designing cloud-native solutions that leverage GCP's comprehensive service ecosystem.

## Purpose

This repository demonstrates technical approaches to designing and implementing systems on Google Cloud Platform that balance performance, cost-efficiency, scalability, and operational excellence. It highlights architectural patterns and best practices for leveraging GCP services to solve real-world challenges across various industries and technical domains.

## Structure

The repository uses a branch-based organization where each case study is self-contained:

- `main`: Contains the overview README and repository documentation
- Case study branches: Each scenario is developed in its own dedicated branch with:
  - Individual README with scenario-specific documentation
  - `.gitignore` for environment-specific exclusions
  - `notebooks/` directory containing the proposal Jupyter notebook
  - `components/` directory with implementation modules, each in their own subdirectory
  - `environment.yml` containing all conda environment specifications for the case study and its components

## Case Studies Overview

| Scenario | Topic | Notebook | Status |
|:--------:|-------|:--------:|:------:|
| 1 | [Healthcare Data Platform Security Architecture](https://github.com/iTrauco/google-cloud-sad/tree/scenario01/healthcare-security/data-platform-iam) | [Proposal Notebook](https://github.com/iTrauco/google-cloud-sad/blob/scenario01/healthcare-security/data-platform-iam/notebooks/%5BDRAFT%5D%20Healthcare%20Security%20Data%20Platform%20IAM%20-%20System%20Analysis%20and%20Design%20Proposal.ipynb) | 🟡 |
| 2 | [Enterprise BigQuery Integration & Governance](https://github.com/iTrauco/google-cloud-sad/tree/scenario02/enterprise-bigquery/integration-governance) | [Proposal Notebook](https://github.com/iTrauco/google-cloud-sad/blob/scenario02/enterprise-bigquery/integration-governance/notebooks/%5BDRAFT%5DEnterprise%20BigQuery%20Integration%20Governance%20-%20System%20Analysis%20and%20Design%20Proposal.ipynb) | ⚫ |
| 3 | [Medical Imaging Processing Pipeline](https://github.com/iTrauco/google-cloud-sad/tree/scenario03/medical-imaging/processing-pipeline) | TBD | ⚫ |
| 4 |  |  |  |
| 5 |  |  |  |
| 6 |  |  |  |
| 7 |  |  |  |
| 8 |  |  |  |
| 9 |  |  |  |
| 10 |  |  |  |
| 11 |  |  |  |
| 12 |  |  |  |
| 13 |  |  |  |
| 14 |  |  |  |
| 15 |  |  |  |
| 16 |  |  |  |
| 17 |  |  |  |
| 18 |  |  |  |
| 19 |  |  |  |
| 20 |  |  |  |

**Status Key:** ⚫ Not Started | 🟡 In Progress | 🟢 Complete | 🔒 On Hold | 🔴 Abandoned