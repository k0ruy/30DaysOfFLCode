# Day 2

Goal: study of [Federated Learning: Challenges, Methods, and Future Directions](https://arxiv.org/pdf/1908.07873) Survey of Related and Current Work

## Survey of Related and Current Work
### Key Concepts and Motivation:

Communication efficiency is a critical aspect of Federated Learning (FL), as frequent communication between devices and servers can cause significant delays and strain network resources. In FL, where a central server coordinates decentralized devices, optimizing the volume and frequency of communication is essential for scalability and practicality. This need arises due to devices having varying connectivity and bandwidth, making traditional communication-heavy methods unsuitable.

### Methods and Techniques:

1. **Local Updating Methods:**
   - Devices perform several local updates using their data before transmitting to the server, reducing the number of communication rounds.
   - Algorithms like Federated Averaging (FedAvg) aggregate updates periodically to balance computational effort and communication demands.

2. **Model Compression Techniques:**
   - Approaches like sparsification, quantization, and subsampling reduce the size of updates sent during each communication round.
   - These techniques mitigate communication costs but must account for FL-specific challenges like data heterogeneity and intermittent client participation.

3. **Decentralized Training:**
   - Instead of relying on a central server, some FL systems distribute the communication burden across a peer-to-peer network.
   - Decentralized topologies reduce server bottlenecks but introduce new complexities in coordination and synchronization.

### Key Challenges:

- **Balancing Trade-offs:** Achieving an optimal trade-off between local computation and communication frequency is difficult, especially with heterogeneous device capabilities.
- **Non-IID Data Impact:** Compression techniques and local updates may exacerbate statistical divergence due to non-identical and non-independent data distributions across devices.
- **Dynamic Participation:** Devices may drop in and out of communication, complicating synchronization and model consistency.

### Vision and Contributions:

This chapter highlights the importance of designing adaptive and resilient communication strategies tailored to the FL setting. It emphasizes the need for:
- Flexible protocols that handle device heterogeneity.
- Robust compression methods that maintain model accuracy despite reduced communication.

>[!TIP]
>**Take-home Message:** Communication efficiency in FL is vital for enabling scalable and practical implementations. While strategies like local updates, compression, and decentralized topologies offer promising solutions, addressing the inherent challenges of heterogeneity and synchronization remains critical for future progress.
