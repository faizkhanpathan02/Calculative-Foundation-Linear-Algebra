# 📊 Calculative Foundation: Linear Algebra in Student Performance Analysis

A complete, production-ready project exploring the mathematical and computational foundations of **Linear Algebra applied to Data Science & AI/ML**.

---

## 🎯 Project Overview
This project analyzes student performance data across multiple academic subjects using linear algebraic structures, vector spaces, matrix transformations, geometric hyperplanes, and eigenvalue decompositions (Principal Component Analysis foundations).

- **Duration:** 6 Hours (Theory + Practical)
- **Domain:** Data Analytics, Applied Mathematics, Machine Learning

---

## 🗂️ Repository Structure

```
├── Calculative_Foundation.ipynb               # Complete Jupyter Notebook with code, plots & explanations
├── Calculative_Foundation_Theory_and_Analysis.pdf # Detailed Academic & Theoretical Report (PDF)
├── student_scores.csv                        # Dataset of 5 students across 5 subjects
├── README.md                                 # Documentation & Submission Guide
```

---

## 📋 Summary of Key Results & Interpretations

### 📌 Part A: Vector Fundamentals
| Operation | Aarav | Bhavya | Interpretation |
| :--- | :--- | :--- | :--- |
| **Norm-1 ($L_1$)** | `433.0` | `362.0` | Represents total aggregate marks across all subjects. |
| **Norm-2 ($L_2$)** | `193.95` | `162.28` | Euclidean magnitude; sensitive to high peak scores. |
| **Dot Product** | `31,256` | — | Scalar measure of collective alignment. |
| **Angle ($\theta$)** | `6.75°` | (Cosine: `0.9931`) | Near zero angle indicates nearly identical subject profiles. |
| **Cross Product (3D)** | `[1350, -1340, 75]` | — | Normal vector orthogonal to Math, Physics & Chemistry plane. |
| **Projection (Aarav on Bhavya)** | `[83.08, 89.02, 94.95, 77.15, 85.46]` | — | Aarav's profile scaled along Bhavya's score trajectory. |

---

### 📌 Part B: Matrix Operations
- **Matrix Dimension:** $5 \times 5$ (5 Students $\times$ 5 Subjects)
- **Determinant:** $\det(A) = 13,125.0 \neq 0$
- **Rank:** Full Rank ($	ext{rank} = 5$).
- **Invertibility:** Yes, $A^{-1}$ exists. Proves that all student profiles are linearly independent (no student is a redundant linear combination of others).

---

### 📌 Part C: Geometry & Hyperplanes
- **Line (1D in $\mathbb{R}^2$):** Models pairwise relationship (e.g., Math vs Physics).
- **Plane (2D in $\mathbb{R}^3$):** Surface formed by 3 subjects (Math, Physics, Chemistry).
- **Hyperplane (4D in $\mathbb{R}^5$):** $w^T x = \sum_{i=1}^5 w_i x_i = b$. Acts as the linear decision boundary dividing student cohorts (e.g., Honors vs Regular) in high-dimensional feature spaces.

---

### 📌 Part D: Eigenvalues & Dimensionality Reduction (PCA)
- **$\lambda_1 = 632.17$ (92.69% variance):** Dominant component representing overall academic ability across all subjects.
- **$\lambda_2 = 44.85$ (6.58% variance):** Secondary component capturing STEM vs Humanities preference.
- **Dimensionality Reduction:** The top 2 components preserve **99.27%** of total variance, allowing 5D student performance data to be represented in 2D with almost zero information loss.

---

## 🚀 How to Run the Notebook
```bash
# Clone the repository
git clone <your-repo-link>
cd <repo-name>

# Install required packages
pip install numpy pandas matplotlib seaborn

# Launch Jupyter
jupyter notebook Calculative_Foundation.ipynb
```
