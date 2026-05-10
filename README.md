<div align="center">

# 🌌 Sujal Parab

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=24&pause=1000&color=00ADD8&center=true&vCenter=true&width=600&lines=Computer+Engineering+%40+DJ+Sanghvi;Building+High-Performance+Systems+in+Go;Seeking+Summer+2026+Backend+Internships" alt="Typing SVG" />

*Engineering highly scalable backend infrastructure, concurrent systems, and AI models.*

</div>

---

### 🛰️ Core Engineering Stack

<div align="center">
  <img src="https://skillicons.dev/icons?i=go,cpp,c,java,python,js,html,css,react,nodejs,express,mongodb,postgres,docker,git&perline=8" />
</div>
### ⚡ Engineering Focus & Trajectory

> *"Building scalable backend architecture, mastering concurrency, and exploring high-performance systems."*

* 🔭 **Currently architecting:** Advanced backend systems using Golang primitives, focusing on high-throughput concurrency and cloud infrastructure.
* 🌱 **Exploring:** Concepts in High-Frequency Trading (HFT), low-latency system design, and integrating Python-based predictive ML models.
* ⚡ **Beyond the code:** I treat system optimization and algorithmic problem-solving like an intellectual sport. When I am taking a break from backend architecture, I am usually studying chess variations.

### 🌐 The 3D Contribution Matrix

<div align="center">

![3D Contribution Graph](./profile-3d-contrib/profile-night-view.svg)

</div>
---

<div align="center">
  📫 <b>Looking for Summer 2026 Internships in Backend / Software Engineering</b>
</div>
### ⚙️ System Architecture: Concurrent Processing Flow

*A conceptual model of a high-throughput validation engine utilizing Golang concurrency primitives.*

```mermaid
sequenceDiagram
    participant Client
    participant Main as Main Thread
    participant WaitGroup as sync.WaitGroup
    participant Workers as Goroutine Pool
    participant Channels as Results Channel

    Client->>Main: Initiate Batch Task
    Main->>WaitGroup: Add(N) Tasks
    Main->>Workers: Dispatch Concurrent Workers
    
    loop Parallel Execution
        Workers->>Workers: Process I/O
        Workers-->>Channels: Send Output Status
        Workers->>WaitGroup: Done()
    end
    
    WaitGroup-->>Main: Wait() triggers completion
    Channels-->>Main: Aggregate Streams
    Main->>Client: Return Optimized Response
