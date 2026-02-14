# 📷 Camera and CAN Integration in ADAS

## 🚗 Overview

This project presents a detailed case study on the integration of automotive camera systems with Controller Area Network (CAN) communication in Advanced Driver Assistance Systems (ADAS). It analyzes how perception data from camera sensors can be processed, encoded, and transmitted efficiently within the bandwidth constraints of CAN Layer 2.

The study combines concepts from computer vision, embedded systems, and automotive networking to evaluate real-time feasibility in modern intelligent vehicles.

---

## 🎯 Objectives

- Understand stereo camera-based distance estimation using disparity
- Analyze CAN Layer 2 net data rate and propagation timing
- Implement signal scaling and physical value conversion
- Design 64-bit PDU mapping for structured object data
- Evaluate feasibility of transmitting camera data over CAN
- Explore multi-modal 3D object detection concepts

---

## 📌 Project Components

### 1️⃣ Stereo Vision & Depth Estimation
- Mathematical derivation of disparity-based depth calculation  
- Example implementation using baseline, focal length, and pixel shift  
- Demonstrates 3D distance estimation for ADAS perception  

### 2️⃣ CAN Layer 2 Analysis
- Gross vs. net data rate calculation  
- Protocol efficiency evaluation  
- Bit timing and propagation delay constraints  
- CAN 2.0 frame structure breakdown  

### 3️⃣ Signal Scaling & PDU Mapping
Linear scaling formula:

Physical Value = Raw Value × Scaling Factor + Offset

- 64-bit CAN frame visualization  
- Bit-level mapping of object detection signals:
  - Object ID
  - Object Classification
  - Height & Width
  - Relative Velocity
  - Lane Position
  - Cut-In Probability

### 4️⃣ Feasibility Study
- ✔ Object Data → Feasible over CAN (compact & structured)
- ❌ Raw Image Data → Not feasible (requires Ethernet or edge processing)

### 5️⃣ Image Processing
- Application of edge detection filter on grayscale image
- Demonstrates lightweight perception preprocessing

### 6️⃣ Multi-Modal 3D Detection (Literature Study)
- Representation, alignment, and fusion taxonomy
- Learning-based vs learning-agnostic fusion methods
- Challenges in real-time deployment

---

## 📊 Key Findings

- CAN Layer 2 supports structured object data transmission.
- Raw camera image data exceeds CAN bandwidth limits.
- Proper signal scaling and bit mapping ensure reliable communication.
- High-resolution sensors require Ethernet-based architectures.
- Multi-modal fusion improves perception accuracy but increases computational demand.

---

## 🛠 Technologies & Concepts

- CAN 2.0 Protocol  
- Automotive Embedded Systems  
- Stereo Vision Mathematics  
- Signal Encoding & Scaling  
- Edge Detection (Convolution Filtering)  
- Multi-Modal Sensor Fusion  

---

## 🎓 Academic Context

Master of Automotive Software Engineering  
Technische Hochschule Deggendorf  

Course: Advanced Driver Assistance Systems (ADAS)

---

## 🔮 Future Scope

- Integration with Automotive Ethernet  
- Edge AI deployment for real-time processing  
- Transformer-based multi-modal fusion  
- Scalable perception architectures for autonomous driving  

---

## 👨‍💻 Author

Deep Bharatbhai Savaliya  
Master’s Student – Automotive Software Engineering  
