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



