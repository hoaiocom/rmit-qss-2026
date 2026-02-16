## About

**RMIT Quantum Summer School 2026** — Hands-on quantum computing labs using **Qiskit 2.x**. This repository contains tutorials and projects on foundational quantum algorithms, with all circuits run on local simulators (ideal and noisy).
- Instructor: Hoa Nguyen

---

## 📁 Repository contents

| File | Description |
|------|-------------|
| **requirements.txt** | Python dependencies (Qiskit, Qiskit Aer, matplotlib, etc.). |
| **tutorials/Tutorial-Deutsch-Algo.ipynb** | **Tutorial:** Deutsch’s algorithm with a 1-qubit oracle. Learn how to decide if a Boolean function is constant or balanced in a single quantum query. |
| **tutorials/Tutorial-Grover-Algo.ipynb** | **Tutorial:** Introduction to Grover’s search algorithm with Qiskit 2.x. |
| **projects/Project-DJ-Algo.ipynb** | **Project:** Generalised **Deutsch–Jozsa** algorithm for *n*-qubit oracles. Implement constant/balanced oracles, analyse phase kickback, circuit depth, and quantum vs classical query complexity. |
| **projects/Project-Grover-Algo.ipynb** | **Project:** **Grover’s search** for *n*-qubit systems. Implement single and multiple marked items, oracles, optimal iteration counts, amplitude amplification analysis, and validation on ideal/noisy simulators. |

---

## 🛠️ Getting Started

You can run the notebooks **on Google Colab** (no local install) or **locally** on your machine.

---

### Option A: Run on Google Colab

1. **Open a notebook in Colab**
   - Go to [github.com/hoaiocom/rmit-qss-2026](https://github.com/hoaiocom/rmit-qss-2026), open the notebook you want (e.g. `Tutorial-Deutsch-Algo.ipynb`), then click **Open in Colab**.
   - Or in [Google Colab](https://colab.research.google.com): *File* → *Open notebook* → *GitHub* and paste the repo URL.

2. **Install dependencies** (run once per session)
   - Add a new cell at the top and run:
   ```python
   !pip install -r https://raw.githubusercontent.com/hoaiocom/rmit-qss-2026/main/requirements.txt
   ```

3. **Run the cells** as usual. All simulations run on Colab’s runtime.

---

### Option B: Local setup

#### 1. Clone the Repository

```bash
git clone https://github.com/hoaiocom/rmit-qss-2026.git
cd rmit-qss-2026
```

#### 2. Environment Setup

**Using venv:**
```bash
python -m venv qss
source qss/bin/activate  # On macOS/Linux
# or
qss\Scripts\activate     # On Windows
```

**Using Conda:**
```bash
conda create -n qss python=3.12
conda activate qss
```

#### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

**Main Dependencies:**
- `qiskit==2.3.0` - Quantum computing framework
- `qiskit-aer==0.17.2` - High-performance quantum circuit simulator
- `qiskit_ibm_runtime==0.45.0` - IBM Quantum runtime services
- `matplotlib==3.10.8` - Plotting and visualization
- `pylatexenc==2.10` - LaTeX encoding support

#### 4. Launch Jupyter Notebook

Navigate to the lab directory and open the desired notebook file.

**Recommended IDEs:**
- [Visual Studio Code](https://code.visualstudio.com/) - Free, powerful code editor with excellent Jupyter notebook support
- [Jupyter Lab](https://jupyter.org/) - Classic notebook environment

## 📝 Working with the Labs

### Notes:

1. **Kernel Management:** If you restart the kernel, re-run all code cells from top to bottom
2. **Pre-filled Code:** Do not modify cells with pre-written code in assignment section if you're unsure
3. **Your Code Areas:** Look for comments like `### WRITE YOUR CODE BELOW THIS CELL ###`
4. **Local Simulation:** Due to regional restrictions, we run quantum simulations locally instead of on IBM's cloud hardware

### Lab Structure:
- **Markdown cells:** Explanations and instructions
- **Code cells:** Hands-on quantum programming exercises
- **Visualization:** Quantum circuit diagrams and result plots

## 📖 Additional Resources

- [IBM Quantum Documentation](https://quantum.cloud.ibm.com/docs/en/guides)
- [IBM Quantum Learning](https://quantum.cloud.ibm.com/learning/en)
- [Python Virtual Environments Guide](https://docs.python.org/3/library/venv.html)
- [Conda Environment Guide](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)