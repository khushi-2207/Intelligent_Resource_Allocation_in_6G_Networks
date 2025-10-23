# 🌐 Resource Allocation Optimization in 6G Networks

**Project Overview:**  
This project focuses on designing an **intelligent, secure, and adaptive resource allocation system** for future 6G networks. By combining **AI-driven scheduling**, **blockchain trust mechanisms**, and **THz spectrum management**, the framework addresses ultra-high data rates, URLLC, eMBB, and mMTC demands while ensuring fairness, scalability, and reliability.

---

## 📄 Abstract

The evolution of 6G networks requires **intelligent, scalable, and secure resource allocation strategies** to handle extreme data demands and diverse QoS requirements. This project proposes a **hybrid framework** integrating **AI-based proportional fair scheduling**, **blockchain-secured transactions**, and **THz spectrum management**. Simulation and theoretical evaluation demonstrate the effectiveness of the system in terms of **throughput, fairness, adaptability, and scalability**.

---

## 📌 Problem Statement

Current LTE and 5G scheduling techniques are insufficient for 6G due to:  
* Ultra-high data rates and spectrum scarcity.  
* Diverse QoS requirements (URLLC, eMBB, mMTC).  
* Dynamic network conditions and user mobility.  

**Objective:**  
Develop a **modular, scalable, and secure resource allocation system** that:  
* Adapts to real-time network conditions.  
* Ensures fairness among users.  
* Leverages AI, blockchain, and THz spectrum capabilities.

---

## 🛠 Methodology

### **4.1 Overview**
* Design an **intelligent and flexible resource allocation system** for 6G.  
* Combines AI, blockchain, and THz spectrum management to enhance performance in dynamic and resource-constrained environments.

### **4.2 AI-Based Proportional Fair Scheduling**
* AI-driven **Proportional Fair (PF) scheduler** adapts scheduling based on:  
  - Traffic history  
  - User mobility  
  - Service class  
  - Channel state  
* Uses **reinforcement learning** to continuously improve throughput, latency, and packet loss.

### **4.3 Cluster-Based Network Design**
* Network divided into clusters controlled by gNodeB and femtocells.  
* Femtocells run **local AI scheduling**, supervised by macro base station for global coordination.  

### **4.4 Blockchain Integration**
* Records all resource allocation transactions in a **distributed ledger**.  
* **Smart contracts** enforce SLAs and prevent malicious actions.  
* Consensus via **PoA and DPoS** ensures efficiency.

### **4.5 THz Spectrum Management**
* THz waves provide high-speed connectivity but have low propagation distance.  
* **THz management module** senses device location, obstacles, and dynamically allocates sub-bands.  

### **4.6 QoS Classifier**
* Traffic categorized as URLLC, eMBB, or mMTC.  
* Ensures **priority allocation** to latency-critical services.  

### **4.7 Modularity and Deployment**
* Modular design supports **urban, rural, and high-mobility environments**.  
* Performance evaluated using **Jain’s Fairness Index, spectral efficiency, energy consumption, and user satisfaction**.

---

## 🏗 System Design

### **5.1 Layered Structure**
* **User & Device Layer:** Smartphones, IoT sensors, autonomous machines, wearables.  
* **Edge & Cluster Management Layer:** Femtocells and cluster controllers with AI scheduling and THz allocation.  
* **Control & Coordination Layer:** Macro base station for blockchain ledger, global AI coordination, and smart contract enforcement.

### **5.2 AI-Based Scheduler**
* Collects data: user location, movement, channel quality, QoS type.  
* Reinforcement learning ensures **real-time adaptation**.  

### **5.3 Blockchain Ledger**
* Logs all resource allocation transactions.  
* Smart contracts automate **SLA enforcement** and **policy compliance**.  

### **5.4 THz Spectrum Module**
* Allocates ultra-high frequency spectrum based on line-of-sight and environment.  
* Works with AI scheduler to optimize throughput and connectivity.

### **5.5 QoS Prioritization**
* Ensures critical services (e.g., autonomous driving, remote surgery) get priority.  
* Best-effort traffic utilizes remaining resources.  

### **5.6 Feedback Loop**
* Continuous performance feedback to AI core.  
* Enables **dynamic adaptation** and improved future scheduling.

### **5.7 Scalability**
* Modular design allows **incremental network deployment** and **future upgrades**.

---

## 🏛 Architecture

### **6.1 Architectural Layers**
1. **User & Device Layer:** Handles service requests and QoS classification.  
2. **Edge & Cluster Management Layer:** AI scheduling, THz allocation, QoS enforcement.  
3. **Control & Coordination Layer:** Blockchain ledger, global AI coordinator, and smart contracts.

### **6.2 Flow of Scheduling**
1. User sends access request with QoS tag.  
2. Edge node profiles device and evaluates channel.  
3. AI scheduler computes PF score.  
4. THz manager selects optimal frequency band.  
5. Scheduler allocates Resource Blocks (RBs).  
6. Blockchain logs the transaction.  
7. Feedback loop updates AI for continuous learning.

### **6.3 Frequency Band Allocation**
* Users assigned **primary band** (THz, mmWave, or sub-6 GHz) and **secondary band** for fallback.  
* Allocation depends on **data rate, latency, device type, and power efficiency**.

---

## 📊 Simulation and Results

### **Simulation Setup**
* 6G microcell environment: 100m × 100m  
* 200 UEs, 25 BSs  
* Path loss: free-space + molecular absorption (κ=0.003) + shadow fading (σ=4 dB)  
* Transmit Power: 30 dBm, Bandwidth: 1 GHz  
* SNR computed using Shannon’s formula

### **Simulation Parameters**

| Parameter                     | Value          |
|--------------------------------|----------------|
| Number of User Equipments (UE) | 200            |
| Bandwidth                       | 1 GHz          |
| Transmit Power                  | 30 dBm         |
| Noise Spectral Density          | 1e-20 W/Hz     |
| Path Loss Exponent (α)          | 2.5            |
| Molecular Absorption Coefficient (κ) | 0.003 1/m |
| Shadow Fading Std Dev (σ)       | 4 dB           |
| Maximum Distance to BS           | 100 meters     |

### **Output Statistics**
* Jain's Fairness Index: 0.2490  
* Average Throughput: 26,126.94 Mbps  
* Max Throughput: 38,875.94 Mbps  
* Min Throughput: 21,499.22 Mbps  

### **Simulation Results**
* Average user throughput: ~0.9 Gbps  
* Jain’s Fairness Index >0.98  
* Dynamic adaptation to channel conditions  
* Scalable up to 50 users maintaining throughput and fairness  
* PFS outperforms Round Robin and Max-Min Fairness

### **Conclusion**
* AI-based PFS effectively balances **throughput and fairness**  
* Dynamic real-time adaptation ensures **robustness** in high-mobility 6G environments  
* Blockchain ensures **trust and transparency**  
* Scalable and modular for **future 6G deployments**  
* Provides a blueprint for **real-world 6G network implementations**

---

## ⚙ Key Technologies
* **Artificial Intelligence (AI)** – Reinforcement learning for scheduling  
* **Blockchain** – Immutable ledger and smart contract enforcement  
* **THz Spectrum Management** – High-speed, low-latency communication  
* **QoS Classification** – URLLC, eMBB, mMTC support  
* **Modular Architecture** – Scalable and adaptable for diverse environments

---

## 🔗 References
* [6G Wireless Networks: Vision and Challenges](#)  
* [Proportional Fair Scheduling and AI Techniques](#)  
* [Blockchain in Wireless Networks](#)  
* [THz Communication Fundamentals](#)

## 📄 Full Project Report

[Download the Project Report PDF](Resource_Allocation_6G_Project_Report.pdf)


