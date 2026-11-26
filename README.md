```mermaid
flowchart TD
    A[NEW] -->|start()| B[RUNNABLE]
    B -->|Lock unavailable| C[BLOCKED]
    C -->|Lock acquired| B
    B -->|wait() / join()| D[WAITING]
    B -->|sleep() / timed wait| E[TIMED_WAITING]
    D -->|Notify / completion| B
    E -->|Time over| B
    B -->|run() completes| F[TERMINATED]

```
---

```mermaid
flowchart TD
    A[NEW] -->|start()| B[RUNNABLE]

    B -->|Lock unavailable| C[BLOCKED]
    C -->|Lock acquired| B

    B -->|wait() / join()| D[WAITING]
    B -->|sleep() / timed wait| E[TIMED_WAITING]

    D -->|Notify / completion| B
    E -->|Time over| B

    B -->|run() completes| F[TERMINATED]

    style A fill:#dbeafe,stroke:#2563eb,color:#1e3a8a
    style B fill:#dcfce7,stroke:#16a34a,color:#14532d
    style C fill:#fef3c7,stroke:#d97706,color:#78350f
    style D fill:#f3e8ff,stroke:#9333ea,color:#581c87
    style E fill:#ffedd5,stroke:#ea580c,color:#7c2d12
    style F fill:#fee2e2,stroke:#dc2626,color:#7f1d1d
```

    
# Data Structures and Algorithms (DSA) in C++ 📚

Welcome to my **DSA course repository**!  
This repository contains `C++ solutions` for various `Data Structures and Algorithms` topics, organized for easy navigation, learning, and practice.

---

## 📂 Repository Structure

- Each folder contains `.cpp` files solving problems related to that topic.  

---

## 💻 How to Use This Repository

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/sumitkumar2374/DSA-course.git

```

## Navigate to the Desired Folder

- `cd` DSA/TopicFolder

## Compile the C++ Code

- `g++ problem.cpp -o problem`

## Run the Executable

- **Windows:**
  - `problem.exe`

- **Linux / Mac:**
  - `./problem`

## 📌 Author

**Mr Sumit Kumar**



