# Week 1: Percolation Theory & Phase Transitions

**Topic:** Numerical Simulation of Site and Bond Percolation  
**Algorithm:** Hoshen-Kopelman with Union-Find  
**Language:** Python (Jupyter Notebook)


## 📊 Analysis & Results
The simulation performs the following analyses (visualizations available in the Notebook and Report):

### 1. Cluster Identification
We implemented the **Hoshen-Kopelman algorithm** to identify connected clusters on $L \times L$ lattices. The code visualizes these clusters to qualitatively demonstrate the difference between non-percolating (low $p$) and percolating (high $p$) states.

### 2. Phase Transition Analysis (Site Percolation)
We calculated Percolation Strength ($P_\infty$), Probability ($\Pi$), and Average Cluster Size ($S$) for lattice sizes $L=8, 16, 32$.
- The intersection of probability curves indicates a critical probability of **$p_c \approx 0.59$**.
- The Average Cluster Size shows a distinct divergence (peak) at the critical point.

### 3. Bond Percolation Comparison
We also simulated Bond Percolation, observing a phase transition at **$p_c \approx 0.50$**, which aligns with theoretical predictions ($1/2$).

---

## 🚀 How to Run
1. Navigate to this folder:
   ```bash
   cd Computational-Physics-MnP/Week1_Percolation
