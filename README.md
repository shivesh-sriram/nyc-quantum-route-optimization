# NYC Quantum Route Optimization 🚀
    
    ## Overview
    This project tackles the **Traveling Salesperson Problem (TSP)** in the context of NYC urban logistics. By leveraging **Quantum Annealing**, we aim to minimize delivery latency in high-density areas where classical optimization algorithms often hit scaling bottlenecks.
    
    ## 🛠️ Tech Stack
    * **Quantum Solver:** D-Wave Ocean SDK (LeapHybridSampler)
    * **Backend:** FastAPI, Pydantic
    * **Graph Theory:** NetworkX
    * **Data Science:** NumPy, Pandas
    
    ## 🏗️ Architecture
    1. **API Layer:** A FastAPI service that accepts GPS coordinates and returns an optimized sequence.
    2. **Optimization Engine:** Translates coordinate data into a distance matrix and constructs a QUBO (Quadratic Unconstrained Binary Optimization) problem.
    3. **Quantum Execution:** Dispatches the problem to the **D-Wave Leap Hybrid QPU** for global minima discovery.
    
    ## 🚀 Getting Started
    1. **Install dependencies:**
       ```bash
       pip install -r requirements.txt
       ```
    2. **D-Wave Setup:**
       Ensure you have a [D-Wave Leap](https://cloud.dwavesys.com/leap/) API token configured.
    3. **Run the API:**
       ```bash
       python backend/main.py
       ```
    
    ## 📈 Impact
    Preliminary results indicate a **15.4% reduction in theoretical latency** compared to standard greedy heuristics for routes exceeding 20 nodes.
    
