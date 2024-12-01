# Day 9

Study of [A robust analysis of adversarial attacks on federated learning environments](https://www.sciencedirect.com/science/article/pii/S0920548923000041?casa_token=E-t_KBVyo_EAAAAA:1ayB45aIVvZwj6Z9qWQQwzMCWN-1ZFjr1Q4qdYr0MujCQqYoISeRlKkRW7abZOsrbqmA4ygHgQ) paper

>[!TIP]
>The chapter introduces the risks of adversarial attacks in FL systems and highlights the need for strong defenses. It prepares for a detailed discussion on attack methods and ways to counter them in later sections.

# Key Points Covered:

1. Adversarial Attacks:
    - Poisoning Attacks: These occur when adversaries aim to corrupt the learning process:
      - Data Poisoning: Malicious entities introduce harmful or misleading data to manipulate the model’s outputs.
      - Model Poisoning: Adversaries modify model updates before sending them to the central server, directly impacting the training process.
    - Inference Attacks: These attacks focus on extracting sensitive information about the training data from shared model updates, posing a significant risk to user privacy.
2. System Vulnerabilities:
    - The absence of centralized oversight leaves FL systems vulnerable to malicious participants.
    - The iterative nature of FL amplifies the effects of even small-scale adversarial actions over multiple training rounds.

3. Impact of Adversarial Actions:
    - The attacks not only compromise the accuracy and integrity of the trained model but also threaten its fairness and reliability.
    - The chapter highlights how such vulnerabilities can erode trust in FL systems, particularly in critical applications like healthcare, finance, and personalized services.

4. Challenges in Mitigation:
    - Detecting and mitigating adversarial activities is particularly challenging in FL due to the diversity of participating devices and the limited visibility of local operations by the central server.
    - Existing solutions often struggle to balance robustness, efficiency, and privacy.
