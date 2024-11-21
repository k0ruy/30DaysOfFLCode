# Day 1

Goal: study of [Federated Learning: Challenges, Methods, and Future Directions](https://arxiv.org/pdf/1908.07873) introduction

## Introduction

**Key Concepts and Motivation:**

Federated Learning (FL) is a distributed machine learning paradigm where models are trained collaboratively across decentralized devices or servers, such as mobile phones or IoT devices, while keeping the data localized to the devices.
Unlike traditional centralized learning, where data is aggregated into a single server, FL emphasizes privacy-preserving model training by avoiding direct access to raw data.
FL aligns with the growing importance of data privacy regulations, like GDPR and HIPAA, and addresses the inefficiencies of centralized approaches in scenarios with vast amounts of data distributed across multiple devices.

**Applications:**

FL is particularly relevant in domains like healthcare (collaborative training across hospitals), finance (privacy-preserving analysis of sensitive customer data), and edge computing (smartphones, IoT).

**Key Challenges:**
1. Communication Efficiency: Synchronizing models across distributed devices involves significant communication overhead.
2. Statistical Heterogeneity: Data on different devices is non-IID (independent and identically distributed) and varies in quantity and quality, complicating model convergence.
3. System Heterogeneity: Devices have different computational, memory, and network capacities.
4. Privacy and Security: Ensuring that the FL system is robust against adversarial attacks while maintaining strict privacy.
5. Incentive Mechanisms: Encouraging participants to cooperate in federated learning without exploiting or free-riding on the system.

**Vision and Contributions:**

The introduction sets the stage for an in-depth exploration of these challenges, discusses current methods to address them, and highlights future research directions.
It emphasizes that FL is crucial for enabling learning on sensitive, distributed datasets while meeting privacy and efficiency requirements.

>[!TIP]
>**Takehome message:** Federated Learning enables collaborative model training across decentralized devices while preserving privacy, but it faces significant challenges like communication inefficiency, data heterogeneity, and system robustness, offering vast opportunities for innovation.
