
# Medical Imaging Processing Pipeline System Design Proposal

> **Note**: This is a personal repository for developing a systematic approach to GCP cloud architecture and systems engineering using information systems analysis and design principles. The source of truth for work completed in this repository is located in the notebook within the `notebooks/` directory, not in this README.

> **Branch Scope**: All work for this project is scoped to the `scenario03/medical-imaging/processing-pipeline` branch only.

This notebook serves as a comprehensive system design proposal, providing the healthcare imaging company with a structured approach to implementing automated medical image processing pipeline architecture for their containerized workload orchestration and metadata analysis requirements.

## Scenario Overview
A healthcare imaging company wants to process and analyze medical images stored in Cloud Storage through automated pipelines using containerized workloads. They need guidance on Kubernetes orchestration, event-driven processing with Cloud Functions, and BigQuery metadata management for their systematic GCP-based approach. This proposal outlines a systems approach for container orchestration, automated processing pipelines, and metadata architecture - including recommendations for scalability and processing reliability.

## Proposal Framework
This Jupyter notebook presents a systems analysis and design approach to the medical imaging processing pipeline challenge. The proposal follows established information systems design principles, emphasizing:
- **Container-First Architecture**: Methodical approach to designing scalable containerized processing workflows with Kubernetes orchestration
- **Event-Driven Processing**: Structured approach to automated pipeline triggers and serverless processing with Cloud Functions
- **Metadata-Centric Design**: Process-oriented approach to comprehensive metadata capture and BigQuery analytics integration
- **Automated Pipeline Reliability**: Comprehensive monitoring, error handling, and workflow optimization for production processing

## System Components
The proposed solution addresses the following key subsystems:
1. **Container Orchestration Architecture**
   - Kubernetes Engine cluster management and scaling
   - Docker container deployment and lifecycle management
2. **Event-Driven Processing Framework**
   - Cloud Storage trigger mechanisms and Cloud Functions integration
   - Automated workflow orchestration and job scheduling
3. **Image Processing Pipeline Infrastructure**
   - Medical image analysis and transformation workflows
   - Containerized processing job management and queuing
4. **Metadata and Analytics Architecture**
   - BigQuery data warehouse for processing metadata and results
   - Data lineage tracking and processing audit trails
5. **Monitoring and Operations Framework**
   - Pipeline performance monitoring and container health checks
   - Resource optimization and error handling systems

## Implementation Considerations
The proposal includes high-level specifications for:
- Recommended technology stack
- System integration points
- Resource requirements
- Core processing pipeline components

## Reproducibility Framework
### Environment Setup

This project uses a Conda environment to manage dependencies for reproducible analysis. Follow these steps to set up the environment:

#### Prerequisites
- Anaconda or Miniconda installed on your system
- Git for cloning the repository

#### Setup Instructions

1. Clone the repository and switch to the feature branch:
   ```bash
   git clone https://github.com/iTrauco/google-cloud-sad.git
   cd google-cloud-sad
   git checkout scenario03/medical-imaging/processing-pipeline
   ```

2. Create the Conda environment:
   ```bash
   conda create -n scenario03-medical-imaging python=3.11 -y
   ```

3. Activate the environment:
   ```bash
   conda activate scenario03-medical-imaging
   ```

4. Install baseline packages:
   ```bash
   conda install -c conda-forge jupyter numpy pandas matplotlib seaborn -y
   pip install google-cloud-storage google-cloud-bigquery google-cloud-functions kubernetes docker google-cloud-logging google-cloud-monitoring
   ```

5. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

6. Access the notebook in your browser via the URL displayed in the terminal