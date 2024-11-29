# Day 6

Goal: Study of [Model aggregation techniques in federated learning: A comprehensive survey](https://www.sciencedirect.com/science/article/pii/S0167739X23003333).

## Key Concepts
1. Federated Learning Overview: FL involves decentralized training where participants (clients) train models locally and send updates (e.g., gradients or model parameters) to a central server for aggregation. This enables privacy-preserving and collaborative learning across multiple entities.

2. Importance of Aggregation Techniques: Aggregation is pivotal in FL for:
   - Ensuring a robust and generalized global model.
   - Handling non-IID (non-independent and identically distributed) data among clients.
   - Mitigating the risks of adversarial attacks on the model update process.

## Model Aggregation Techniques
The survey categorizes aggregation techniques into three main types based on their focus:

1. Basic Aggregation Techniques:
   - Federated Averaging (FedAvg): The most common technique, which computes a weighted average of local models based on the number of samples at each client.
   - FedProx: Modifies FedAvg to include a regularization term, addressing disparities in data distribution and computational resources among clients.
   - Clustered FL: Groups clients with similar data distributions to improve aggregation accuracy.

3. Robust Aggregation Techniques: Designed to counter adversarial behaviors and model poisoning attacks:
   - Krum: Selects the update closest to most other updates, ignoring outliers.
   - Trimmed Mean and Median: Removes extreme values from updates to prevent malicious data from dominating the global model.
   - Byzantine Robust Methods: Handle updates from faulty or adversarial clients through mechanisms like anomaly detection.

3. Privacy-Preserving Aggregation Techniques:
   - Differential Privacy (DP): Introduces noise into updates before aggregation to protect individual client data.
   - Secure Aggregation: Ensures updates are encrypted during transmission and aggregation.
   - Homomorphic Encryption: Allows computations to occur directly on encrypted updates, enhancing security without compromising utility.
