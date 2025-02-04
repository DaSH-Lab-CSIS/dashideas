# DaSH Lab | Google Summer of Code 2025 - Potential Projects

This page provides an overview of possible projects for GSoC 2025, along with the initial steps and prerequisites required before starting a project.

## Getting started with contributing to DaSH Lab
The GSoC application process involves the following steps:

- Join our [public Slack server](#) and engage in the #gsoc channel to interact with the community.
- Go through the [GSoC Guide for Students](https://developers.google.com/open-source/gsoc/resources/guide) to understand the various stages of the program. This [blog post](#) will also provide additional insights into the application process.
- Review the [GSoC Contribution Timeline](https://developers.google.com/open-source/gsoc/timeline) to stay on track with key dates.
- Familiarize yourself with our [Contributing Guidelines](./CONTRIBUTING.md) to understand the process of contributing to DaSH Lab projects.
- Prepare and submit your application or proposal, including all necessary documentation, through the Google Summer of Code site.
- Remember to reach out to the project mentors for feedback and guidance on your proposal before the application deadline.

## Applying to DaSH Lab for GSoC 2025

The GSoC application process has several stages. First, make sure you meet the [eligibility requirements](https://summerofcode.withgoogle.com/get-started), such as being at least 18 years old and eligible to work in your country of residence. Once you’ve verified eligibility, reach out to the project mentors. The best way to do this is through the `#gsoc` channel on our [Project Discord Server](#), where you can ask questions and share your draft proposals for feedback. Convince your potential mentors that you’re a good fit for the project by demonstrating your previous work, showcasing your relevant skills and experience, and asking insightful questions. 
Finally, submit your project proposal via the GSoC contributor dashboard. 

Note that working on a project could potentially lead to a publication or a conference presentation. 

### Drafting a Proposal
When drafting your proposal, make sure to include the following sections:
- **Project Description**: Provide a detailed description of the project you wish to work on. You can choose a topic from the list below or propose an idea that aligns with the goal of strengthening the [Project Name] ecosystem.
- **Technical Solution Proposal**: Outline your planned approach, including your methodology and technical solution. The more detailed, the better.
- **Project Timeline**: Provide a realistic schedule with clear objectives (e.g., bi-weekly goals) and deadlines, highlighting mid-term and final evaluation milestones.

Ensure to tailor your proposal to the specific project you’re applying for and demonstrate your understanding of the project’s requirements and objectives. Furthermore, make sure to highlight your relevant skills, experience, and contributions to open-source projects.
Research experience, coding skills, and familiarity with a project’s codebase are all valuable assets that can help you stand out as a candidate. Ensure to talk to the project mentors and community members to get feedback on your proposal and improve it before the application deadline.

## Projects for GSoC 2025

- [Hermes++](#hermes++)
- [Reconfiguring Architectures on GPUs](#reconfiguring-architectures-on-gpus)
- [Dynamic Memory Realignment on GPUs](#dynamic-memory-realignment-on-gpus)
- [Static Analyzer for Diamond Pattern Smart Contracts](#static-analyzer-for-diamond-pattern-smart-contracts)
- [Monitoring Dashboard for FL with Flower Framework](#monitoring-dashboard-for-fl-with-flower-framework)
- [UnifyFL - Privacy Preserving Techniques](#unifyfl---privacy-preserving-techniques)
- [Intelligent Pooling in Beegfs](#intelligent-pooling-in-beegfs)
- [Framework for LLM Inference Scheduling for Edge Clusters](#framework-for-llm-inference-scheduling-for-edge-clusters)
- [I/O Simulator for Fog/Edge Simulators](#io-simulator-for-fogedge-simulators)

Note that you can come up with research ideas / engineering projects that align with the goals of the DaSH Lab. Feel free to reach out to the organization admins on Slack to discuss your ideas and get feedback.

---
### Hermes++
**Mentors**: [Advik Raj Basani](#)

**Skills required**: PyTorch, Distributed Systems, Machine Learning

**Rating of the project (Easy / Medium / Hard)**: Medium

Distributed Machine Learning (DML) on edge devices faces significant challenges, including slow convergence and communication overhead, due to the [heterogeneous nature of edge environments](https://www.iiconsortium.org/news-pdf/joi-articles/2021_June_JoI_Edge_Hetero_Compute_Byers_Final.pdf). In this [paper](https://arxiv.org/pdf/2410.20495), a novel probabilistic framework, Hermes, is proposed to address these issues. Hermes reduces communication overhead by transmitting model updates only when significant improvements in generalization are detected, and optimizes dataset allocation to avoid performance degradation caused by straggler nodes. A major assumption in the paper is the time complexity equation (Equation 3), which assumes constant time for ML operations across all tasks. However, this assumption does not necessarily hold for certain workloads, such as [Graph Neural Networks (GNNs)](https://neptune.ai/blog/graph-neural-network-and-some-of-gnn-applications), where the computation time can vary significantly. Additionally, Hermes is currently supported for TensorFlow, but we hope to aim for broader implementation for PyTorch.

**Expected outcomes**:
- An extended implementation of Hermes supporting PyTorch, enabling broader applicability for various ML tasks and enhancing interoperability across frameworks.
- Evaluation of Hermes on diverse workloads, particularly GNNs, to assess the framework’s scalability and effectiveness in resource-constrained edge environments.
- Optimization of the time complexity equation in Hermes to account for varying computation times across tasks, ensuring accurate performance predictions. This is where majority of the research will be focused on.

---
### Reconfiguring architectures on GPUs
**Mentors**: [Advik Raj Basani](#), [Arnab K. Paul](#)

**Skills required**: GPU Architecture, Machine Learning, Distributed Systems

**Rating of the project (Easy / Medium / Hard)**: Hard

Current GPU architectures are engineered as fixed-function accelerators, optimized at design time for broad classes of workloads but unable to adapt to rapidly shifting computational demands or environmental conditions at runtime. This project asks the bold question: “Can we design a GPU system that autonomously reconfigures its microarchitecture in real time to optimize performance, energy efficiency, and fault resilience across diverse and unpredictable workloads?”

**Expected outcomes**:
- A novel GPU architecture that can dynamically reconfigure its microarchitecture at runtime to optimize performance, energy efficiency, and fault resilience across diverse workloads.
- A comprehensive evaluation of the proposed architecture on a range of machine learning, scientific computing, and data analytics workloads to demonstrate its effectiveness and versatility.

---
### Dynamic memory realignment on GPUs
**Mentors**: [Advik Raj Basani](#), [Arnab K. Paul](#)

**Skills required**: GPU Architecture

**Rating of the project (Easy / Medium / Hard)**: Hard

Modern GPUs have become critical components for a wide range of computational tasks, but they still struggle with inefficiencies caused by latent memory redundancies. These redundancies arise from unnecessary duplication and improper data handling within memory, which leads to performance losses. While existing techniques focus on [mitigating redundancies in registers or caches](https://yonsei.elsevierpure.com/en/publications/shreg-mitigating-register-redundancy-in-gpus), memory-level redundancies remain largely unaddressed. The question driving this research is: **Can we develop a system that dynamically identifies and eliminates memory redundancies in real time, optimizing memory usage without manual intervention?**

**Expected outcomes**:
- A novel GPU architecture that dynamically realigns memory to optimize memory usage, reduce redundancies, and improve performance across diverse workloads.
- A comprehensive evaluation of the proposed architecture on a range of machine learning, scientific computing, and data analytics workloads to demonstrate its effectiveness and versatility.

---
### Static Analyzer for Diamond Pattern Smart Contracts
**Mentors**: [?]()

**Skills required**: 

**Rating of the project (Easy / Medium / Hard)**:


**Expected outcomes**:

---
### Monitoring Dashboard for FL with Flower Framework
**Mentors**: [?]()

**Skills required**:

**Rating of the project (Easy / Medium / Hard)**:


**Expected outcomes**:

---
### UnifyFL - Privacy Preserving Techniques
**Mentors**: [?]()

**Skills required**:

**Rating of the project (Easy / Medium / Hard)**:


**Expected outcomes**:

---
### Intelligent Pooling in Beegfs
**Mentors**: [?]()

**Skills required**:

**Rating of the project (Easy / Medium / Hard)**:


**Expected outcomes**:

---
### Framework for LLM Inference Scheduling for Edge Clusters
**Mentors**: [?]()

**Skills required**:

**Rating of the project (Easy / Medium / Hard)**:


**Expected outcomes**:

---
### I/O Simulator for Fog/Edge Simulators
**Mentors**: [?]()

**Skills required**:

**Rating of the project (Easy / Medium / Hard)**:


**Expected outcomes**:

---
