# Linear Algebra for ML — FAANG-Level Lab

**Goal:** Build interview-grade intuition for vectors/matrices, norms, projections, eigenvalues, and SVD — and connect them to ML (least squares, PCA, embeddings).

**Outcome:** Students can compute linear algebra quantities in NumPy, reason about shapes, and explain *why* each concept matters in ML systems.

---

# How to Start

1. **Fork** this repository.  
2. Open `linalg_student_lab.ipynb` in **Google Colab**.  
3. Complete all **TODO** sections.  
4. **Restart runtime → Run All** cells.  
5. Push changes and submit a **Pull Request**.  

⚠️ **Do NOT edit notebooks directly on GitHub.**

---

## Lab Rules (FAANG Style)

- ✅ Always track shapes (write them down)
- ✅ Prefer vectorized operations
- ✅ Validate with sanity checks (orthogonality, reconstruction error)
- ✅ Explain prompts in short bullets

---

# Out of Scope

- Full proof-heavy math
- Deep numerical linear algebra theory

---

# Notebook Rules

- Do **NOT** rename the notebook  
- Do **NOT** delete TODOs  
- Do **NOT** hardcode outputs  
- Notebook must run **top-to-bottom**  

---

# Dataset

- Synthetic matrices/vectors only

## Why?

- Keeps focus on math + computation
- Mirrors interview settings

---

## Section 1 — Vectors, Dot Product, Norms

### Task 1.1: Implement dot + L2 norm

**Checkpoint Questions:**

- What does dot product represent geometrically?
- Why is L2 norm used in least squares?

---

## Section 2 — Matrix Multiplication + Shapes

### Task 2.1: Matmul with shape checks

**FAANG Gotcha:**

- Most ML bugs are silent shape bugs—assert shapes.

---

## Section 3 — Projections

### Task 3.1: Project v onto u

**Interview Angle:**

- Projection is “closest point in a subspace” → least squares intuition.

---

## Section 4 — Least Squares (Closed Form)

### Task 4.1: Solve normal equations with `np.linalg.solve`

**FAANG Gotcha:**

- Avoid explicit inverse; solve is more stable and faster.

---

## Section 5 — Eigenvalues & SVD (PCA)

### Task 5.1: PCA via SVD + reconstruction error

**Checkpoint Questions:**

- Why does SVD show up in embeddings and compression?
- What does reconstruction error measure?

---

## Submission Expectations

Students must submit:

- Clean notebook (runs top-to-bottom)
- Answers to **Checkpoint/Explain** prompts
- Sanity checks passing

---

## FAANG Interview Evaluation Rubric

| Skill                    | Evaluated |
|--------------------------|-----------|
| Shape reasoning          | ✅        |
| Correctness              | ✅        |
| Numerical stability      | ✅        |
| ML intuition             | ✅        |
| Explanation clarity      | ✅        |

---

## Stretch

- Implement Gram–Schmidt
- Implement power iteration
- Show PCA via SVD on a small real dataset (optional)
