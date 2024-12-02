# Day 10

Study of [A robust analysis of adversarial attacks on federated learning environments](https://www.sciencedirect.com/science/article/pii/S0920548923000041?casa_token=E-t_KBVyo_EAAAAA:1ayB45aIVvZwj6Z9qWQQwzMCWN-1ZFjr1Q4qdYr0MujCQqYoISeRlKkRW7abZOsrbqmA4ygHgQ) paper


>[!TIP]
>Federated learning faces a variety of sophisticated adversarial attacks, but existing defense mechanisms like robust aggregation and anomaly detection provide some protection. However, challenges such as scalability, non-IID data, and adaptive adversaries mean there is still a pressing need for innovative and resilient solutions to secure FL systems effectively.

# Key Topics Covered:

1. Adversarial Attack Strategies:
    - Label-Flipping Attacks: Malicious clients intentionally mislabel data (e.g., changing labels from class A to class B) to corrupt the global model's performance.
    - Backdoor Attacks: Attackers embed hidden triggers within the model, causing it to behave incorrectly when specific conditions are met.
    - Model Poisoning Attacks: Compromised clients send manipulated model updates to the server, aiming to degrade the overall model's accuracy.

2. Defense Mechanisms:
    - Robust Aggregation Techniques: Methods like Krum and Trimmed Mean are designed to mitigate the impact of malicious updates by considering only a subset of client updates during aggregation.
    - Anomaly Detection: Identifying and excluding anomalous updates that deviate significantly from the majority to protect the global model's integrity.
    - Differential Privacy: Adding controlled noise to updates to preserve privacy and reduce the influence of any single client's data.

3. Challenges in Defense Implementation:
    - Scalability: Ensuring defense mechanisms remain effective as the number of clients increases.
    - Non-IID Data Distributions: Addressing the difficulty of distinguishing between malicious updates and legitimate updates from clients with diverse data distributions.
    - Adaptive Adversaries: Developing defenses that can adapt to evolving attack strategies employed by adversaries.
