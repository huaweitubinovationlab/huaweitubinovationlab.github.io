---
title: Projects
subtitle: List of Projects
---

### 2024 - 2025 CloudMap

CloudMap is a graph database and visualization platform developed by the Huawei Cloud SRE team. It stores all the topology relationships within the cloud infrastructure. The main objective of the project was to design an algorithm for root cause analysis using observation data from CloudMap.

As part of the project, a survey of related work in the field of metric-based root cause analysis was conducted. Based on this research, a metric-based RCA algorithm was designed to enable fast and precise localization of anomalies. Additionally, a proposal for incorporating a learning-based approach to root cause analysis for CloudMap was delivered.

**Resources:** 
* [Presentations](https://tubcloud.tu-berlin.de/s/XiZK3px36tKfGwa?path=%2F03_cloud-map-rca%2Fpresentations)
* [Deliverables](https://tubcloud.tu-berlin.de/s/XiZK3px36tKfGwa?path=%2F03_cloud-map-rca%2Fdeliverables)


### 2022 - 2023 Memory Failure Prediction 
The focus of this part of the projects are the failure prediction in RAMs. Large-scale data centers face reliability issues due to memory failures, particularly Uncorrectable Errors (UEs) in Dual Inline Memory Modules (DIMMs), which can lead to data loss and system crashes. Existing prediction models primarily use Correctable Errors (CEs) but fail to account for variations in CPU architectures, such as X86 and ARM, and their different Error Correction Code (ECC) implementations.

This project analyzes the relationship between CEs and UEs across different processors, identifying unique failure patterns for each platform. We focused on applying Machine Learning (ML) and Deep Learning (DL) techniques to real-world production datasets on derived insights from the error patterns. Several innovations were propsed. A key innovation of this research is considering long-term CE history rather than a fixed observation window. Traditional methods analyze recent CEs within limited timeframes, overlooking long-range dependencies. The proposed approach incrementally calculates novel features that preserve long-term trends without excessive storage requirements. This enhances predictive accuracy, enabling failure anticipation up to three hours in advance. Furthermore, an MLOps framework is introduced to continuously enhance prediction performance in live environments. We also proposed a prototypical 3D CNN convolution network approach that aims to combine the streams from the CE and predict anticipating failures. Evaluations on real-world cloud server failures validate the practicality and effectiveness of the proposed innovations.

**Resources:**
* [Presentations](https://tubcloud.tu-berlin.de/s/XiZK3px36tKfGwa?path=%2F02_memory-failure-prediction%2Fpresentations)
* [Deliverables](https://tubcloud.tu-berlin.de/s/XiZK3px36tKfGwa?path=%2F02_memory-failure-prediction%2Fdeliverables)

### 2021 - 2022 Enhancing IT Operations with Intelligent Log Analysis
Log messages serve as a vital link between developers and system operators, yet the lack of standardized guidelines can lead to confusion and inefficiencies in their analysis. To improve this, we developed automated methods for assessing the quality of log instructions, ensuring that log levels are appropriately assigned and that messages provide sufficient detail for effective troubleshooting. By leveraging data-driven techniques, our approach enhances the clarity and usefulness of log messages, facilitating smoother IT operations. 

While the methods devised in the former project enabled us to improve the quality of the logs, it did not address the issue of actually analysis of the logs in operation. To that end techniques for anomaly detection in log data that address semantic and sequential properties of the logs were devised. The former method focusess on utilizing a diverse set of log instructions from a broad range of software projects (1000+) to build a foundational model of log instructions, that is later used in identifying failures in operation. Besides the foundational log model, this method reduces reliance on predefined labels, making anomaly detection more practical and adaptable across different IT environments.

While the former method can address certain issues that are actually logged, it can also miss some failures (e.g., when establishing TCP connection), as the failures reflect in the changed sequence of logs. To address this, we introduce an approach that reinterprets log sequences as sequence of high order chunks of time intervals to extract meaningful operational patterns. By focusing on the context of log events rather than individual occurrences, this method enhances failure identification, allowing for more effective issue resolution and improving overall system stability.

**Resources:** 
* [Presentations](https://tubcloud.tu-berlin.de/s/XiZK3px36tKfGwa?path=%2F01_intelligent-log-analysis%2Fpresentations)
* [Deliverables](https://tubcloud.tu-berlin.de/s/XiZK3px36tKfGwa?path=%2F01_intelligent-log-analysis%2Fcode)
