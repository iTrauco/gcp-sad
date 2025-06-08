# Healthcare Data Platform Security Architecture System Design Proposal

> **Note**: This is a personal repository for developing a systematic approach to GCP cloud architecture and systems engineering using information systems analysis and design principles. The source of truth for work completed in this repository is located in the notebook within the `notebooks/` directory, not in this README.

> **Branch Scope**: All work for this project is scoped to the `scenario01/healthcare-security/data-platform-iam` branch only.

This notebook serves as a comprehensive system design proposal, providing the healthcare technology company with a structured approach to implementing secure data analytics platform architecture for their sensitive patient data analysis requirements.

## Table of Contents
- [Scenario Overview](#scenario-overview)
- [Proposal Framework](#proposal-framework)
- [System Components](#system-components)
- [Implementation Considerations](#implementation-considerations)
- [Reproducibility Framework](#reproducibility-framework)
  - [Environment Setup](#environment-setup)
  - [Prerequisites](#prerequisites)
  - [Setup Instructions](#setup-instructions)
  - [Environment Details](#environment-details)
  - [Environment Management](#environment-management)

## Scenario Overview
A healthcare technology company wants to build a secure data analytics platform using containerized workloads and Cloud Storage for sensitive patient data analysis. They need guidance on Kubernetes security architecture, Docker container protection, Cloud Functions access controls, and BigQuery compliance integration for their systematic GCP-based approach. This proposal outlines a systems approach for container security, serverless access controls, and data platform compliance - including recommendations for scalability and regulatory adherence.

## Proposal Framework
This Jupyter notebook presents a systems analysis and design approach to the healthcare data platform security challenge. The proposal follows established information systems design principles, emphasizing:
- **Security-First Design**: Methodical approach to implementing defense-in-depth security architecture with proper access controls
- **Compliance Integration**: Structured approach to embedding HIPAA and healthcare regulatory requirements into system design
- **Automated Governance**: Process-oriented approach to continuous monitoring, auditing, and compliance validation
- **Observable Security**: Comprehensive monitoring and alerting framework for access patterns and security events

# Scenario 01 - Updated System Components

## System Components
The proposed solution addresses the following key subsystems:
1. **Container Security Architecture**
   - Kubernetes RBAC and cluster security controls
   - Docker container security and image scanning
2. **Data Security and Storage Framework**
   - Cloud Storage encryption and access controls
   - BigQuery data governance and compliance monitoring
3. **Serverless Security Infrastructure**
   - Cloud Functions access controls and authentication
   - Event-driven security monitoring and response
4. **Identity and Access Management (IAM) Subsystem**
   - Role-based access control architecture
   - Privilege management and least-privilege enforcement
5. **Monitoring and Observability Framework**
   - Container and serverless security monitoring
   - Compliance dashboards and audit reporting

## Implementation Considerations
The proposal includes high-level specifications for:
- Recommended technology stack
- System integration points
- Resource requirements
- Core security architecture components

## Reproducibility Framework
### Environment Setup

This project uses a Conda environment to manage dependencies for reproducible analysis. Follow these steps to set up the environment:

#### Prerequisites
- Anaconda or Miniconda installed on your system
- Git for cloning the repository

#### Setup Instructions

1. Clone the repository and switch to the feature branch:
   ```bash
   git clone https://github.com/iTrauco/gcp-sad.git
   cd gcp-sad
   git checkout scenario01/healthcare-security/data-platform-iam
   ```

2. Create the Conda environment:
   ```bash
   conda create -n scenario01-healthcare-security python=3.11 -y
   ```

3. Activate the environment:
   ```bash
   conda activate scenario01-healthcare-security
   ```

4. Install baseline packages:
   ```bash
   conda install -c conda-forge jupyter numpy pandas matplotlib seaborn -y
   pip install google-cloud-iam google-cloud-storage google-cloud-logging google-cloud-monitoring google-cloud-secret-manager google-cloud-kms
   ```

5. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

6. Access the notebook in your browser via the URL displayed in the terminal

#### Environment Details

The environment includes essential data science and security packages:
- [Python 3.11](https://www.python.org/downloads/release/python-3110/)
- [Jupyter Notebook](https://jupyter.org/documentation)
- [pandas](https://pandas.pydata.org/docs/) & [numpy](https://numpy.org/doc/stable/) for data manipulation
- [matplotlib](https://matplotlib.org/stable/index.html) & [seaborn](https://seaborn.pydata.org/) for visualization
- [Google Cloud IAM](https://cloud.google.com/iam/docs) for identity and access management
- [Google Cloud Storage](https://cloud.google.com/storage/docs) for secure data storage
- [Google Cloud Logging](https://cloud.google.com/logging/docs) for audit trail management
- [Google Cloud Monitoring](https://cloud.google.com/monitoring/docs) for security observability
- [Google Cloud Secret Manager](https://cloud.google.com/secret-manager/docs) for secrets management
- [Google Cloud KMS](https://cloud.google.com/kms/docs) for encryption key management

#### Environment Management

For collaborators who enhance the environment with additional packages:

```bash
# Export the updated environment
conda activate scenario01-healthcare-security
conda env export > environment.yml
```