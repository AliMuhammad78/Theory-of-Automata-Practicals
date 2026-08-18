# 🤖 Theory of Automata Practicals

<p align="center">

  <h1 align="center">⚙️ Theory of Automata & Computation</h1>

  <p align="center">
    A collection of practical implementations and study resources covering
    <strong>Finite Automata, Formal Languages, Pushdown Automata, Chomsky Normal Form, and Turing Machines</strong>.
  </p>

  <p align="center">
    <img src="https://img.shields.io/badge/Python-Programs-3776AB?style=for-the-badge&logo=python&logoColor=white">
    <img src="https://img.shields.io/badge/Jupyter-Notebooks-F37626?style=for-the-badge&logo=jupyter&logoColor=white">
    <img src="https://img.shields.io/badge/Automata-Theory-8A2BE2?style=for-the-badge">
    <img src="https://img.shields.io/badge/Formal-Languages-2E8B57?style=for-the-badge">
    <img src="https://img.shields.io/badge/Computation-Theory-orange?style=for-the-badge">
  </p>

</p>

---

## 📚 About The Repository

**Theory of Automata Practicals** is a collection of practical implementations and academic resources developed while studying **Theory of Automata / Theory of Computation** at university.

The repository focuses on converting important theoretical concepts from automata theory and formal languages into **working Python implementations using Jupyter Notebooks**.

The practical work follows a progression from simpler finite-state models toward more powerful computational models:

```text
Finite Automata
      ↓
NFA → DFA
      ↓
DFA Minimization
      ↓
DFA Operations
      ↓
Formal Languages
      ↓
Chomsky Normal Form
      ↓
Pushdown Automata
      ↓
Turing Machines
```

The repository therefore serves both as a **practical programming collection** and as a reference for revising important concepts from the Theory of Automata course.

---

## 🎯 Learning Objectives

The main purpose of this repository is to develop a practical understanding of:

* 🤖 Finite automata
* 🔄 NFA to DFA conversion
* ✂️ DFA minimization
* 🔗 Operations on finite automata
* 🧩 Formal languages
* 📐 Context-Free Grammars
* 🔤 Chomsky Normal Form
* 📚 Pushdown Automata
* 🧠 Turing Machines
* 💻 Computational models

The implementations help connect the mathematical and theoretical concepts of automata with actual algorithms and programs.

---

# 🧠 Practical Implementations

## 01 — NFA to DFA Conversion

📓 `01_nfa_to_dfa.ipynb`

This notebook focuses on converting a **Nondeterministic Finite Automaton (NFA)** into an equivalent **Deterministic Finite Automaton (DFA)**.

### Concepts Covered

* NFA representation
* DFA representation
* States and transitions
* Transition functions
* Subset construction
* Equivalent automata

### Conceptual Flow

```text
       NFA
        │
        ▼
  Subset Construction
        │
        ▼
       DFA
```

The implementation demonstrates how multiple possible NFA states can be represented as a single DFA state.

---

## 02 — DFA Minimization

📓 `02_dfa_minimization.ipynb`

This notebook focuses on reducing a DFA into an equivalent DFA with fewer states.

### Concepts Covered

* Equivalent states
* State partitioning
* Distinguishable states
* Reachability
* DFA reduction
* Minimal DFA

### Conceptual Flow

```text
Original DFA
     │
     ▼
Identify Equivalent States
     │
     ▼
Partition States
     │
     ▼
Merge Equivalent States
     │
     ▼
Minimized DFA
```

The goal is to preserve the language recognized by the DFA while reducing unnecessary states.

---

## 03 — DFA Operations

📓 `03_dfa_operations.ipynb`

This notebook explores operations that can be performed on deterministic finite automata.

Depending on the implementation, automata can be combined to represent operations such as:

* Union
* Intersection
* Difference
* Complement
* Product construction

### Conceptual Representation

```text
DFA A ─────┐
           ├──► Automata Operation ──► Result DFA
DFA B ─────┘
```

These operations demonstrate how new regular languages can be constructed from existing ones.

---

## 04 — Chomsky Normal Form

📓 `04_chomsky_normal_form.ipynb`

This notebook focuses on transforming a **Context-Free Grammar (CFG)** into **Chomsky Normal Form (CNF)**.

CNF provides a standardized structure for context-free grammars and is particularly important in theoretical computer science and parsing algorithms.

### General CNF Structure

Productions generally take forms such as:

```text
A → BC
A → a
```

with special handling for the start symbol where required.

### Transformation Flow

```text
Context-Free Grammar
        │
        ▼
Remove Unnecessary Productions
        │
        ▼
Transform Productions
        │
        ▼
Chomsky Normal Form
```

---

## 05 — Pushdown Automata

📓 `05_pushdown_automata.ipynb`

This notebook introduces **Pushdown Automata (PDA)**, a computational model that extends finite automata with a stack.

A PDA is particularly useful for recognizing **Context-Free Languages**.

### PDA Components

```text
             ┌──────────────┐
Input ──────►│     PDA      │
             │              │
             │  Finite      │
             │  Control     │
             │      +       │
             │    Stack     │
             └──────────────┘
```

### Key Concepts

* States
* Input alphabet
* Stack alphabet
* Transition function
* Stack operations
* Acceptance conditions
* Context-Free Languages

The notebook provides a practical perspective on how a stack enables an automaton to recognize languages that cannot be handled by ordinary finite automata.

---

## 06 — Turing Machines

📓 `06_turing_machines.ipynb`

This notebook explores **Turing Machines**, one of the fundamental mathematical models of computation.

Unlike finite automata and PDAs, a Turing Machine has a tape that can be read and modified during computation.

### Basic Model

```text
          ┌───────────────────────────────┐
          │                               │
          ▼                               ▼
     ┌─────────┐
     │  State  │
     └────┬────┘
          │
          ▼
   ┌─────────────────────────────┐
   │  Tape                       │
   │  0  1  1  0  1  B  B  B     │
   │           ▲                 │
   │         Head                │
   └─────────────────────────────┘
```

### Concepts Covered

* States
* Tape alphabet
* Input alphabet
* Transition function
* Read/write operations
* Head movement
* Accepting states
* Computational processes

Turing Machines provide a theoretical model for understanding the limits and capabilities of computation.

---

# 🗂️ Repository Structure

```text
Theory-of-Automata-Practicals/
│
├── 📁 code/
│   │
│   ├── 01_nfa_to_dfa.ipynb
│   ├── 02_dfa_minimization.ipynb
│   ├── 03_dfa_operations.ipynb
│   ├── 04_chomsky_normal_form.ipynb
│   ├── 05_pushdown_automata.ipynb
│   └── 06_turing_machines.ipynb
│
└── 📁 files/
    │
    ├── Assignment#2 TOA_F25.pdf
    ├── Non-Regular Languaes.ppt.pdf
    └── Toafl-Assignment-2.pdf
```

---

# 📓 Notebook Overview

| #  | Notebook                       | Main Concept        |
| -- | ------------------------------ | ------------------- |
| 01 | `01_nfa_to_dfa.ipynb`          | NFA → DFA           |
| 02 | `02_dfa_minimization.ipynb`    | DFA Minimization    |
| 03 | `03_dfa_operations.ipynb`      | DFA Operations      |
| 04 | `04_chomsky_normal_form.ipynb` | Chomsky Normal Form |
| 05 | `05_pushdown_automata.ipynb`   | Pushdown Automata   |
| 06 | `06_turing_machines.ipynb`     | Turing Machines     |

---

# 📁 Supporting Course Material

The `files` directory contains additional academic resources related to the Theory of Automata course.

### 📄 Included Resources

* **Assignment #2** — Course assignment material
* **Non-Regular Languages** — Presentation/reference material
* **TOAFL Assignment** — Additional assignment material

These resources complement the practical implementations contained in the `code` directory.

---

# 🧩 Core Concepts Covered

## 🤖 Finite Automata

* NFA
* DFA
* State transitions
* Transition functions
* Accepting states
* Subset construction
* DFA minimization
* DFA operations

## 📚 Formal Languages

* Regular languages
* Non-regular languages
* Context-Free Languages
* Formal grammars

## 🌳 Context-Free Grammars

* CFG representation
* Grammar transformations
* Chomsky Normal Form

## 📦 Pushdown Automata

* Stack-based computation
* PDA transitions
* Context-Free Languages
* Acceptance mechanisms

## 🧠 Turing Machines

* Tape
* Head movement
* States
* Transition functions
* Read/write operations
* Computational models

---

# 🗺️ Theory Progression

One of the most important ideas in automata theory is that different computational models have different expressive capabilities.

```text
                    COMPUTATIONAL MODELS
                           │
          ┌────────────────┼────────────────┐
          ▼                ▼                ▼
   Finite Automata       PDA          Turing Machine
          │                │                │
          ▼                ▼                ▼
 Regular Languages   Context-Free     More General
                     Languages        Computation
```

This repository follows that progression practically:

```text
NFA
 │
 └──► DFA
       │
       ├──► Minimization
       │
       └──► Operations
       
CFG
 │
 └──► Chomsky Normal Form
       │
       ▼
      PDA
       
General Computation
       │
       ▼
 Turing Machine
```

---

# 🛠️ Technologies Used

<p align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square\&logo=python\&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square\&logo=jupyter\&logoColor=white)

</p>

### 🐍 Python

Used to implement the algorithms and computational models.

### 📓 Jupyter Notebook

Used for interactive development, demonstrations, experimentation, and documenting the practical implementations.

---

# 🎓 Learning Outcomes

After completing these practical implementations, the following concepts can be practiced and reinforced:

* ✅ NFA and DFA construction
* ✅ NFA-to-DFA conversion
* ✅ DFA minimization
* ✅ DFA operations
* ✅ Regular and non-regular languages
* ✅ Context-Free Grammars
* ✅ Chomsky Normal Form
* ✅ Pushdown Automata
* ✅ Stack-based computation
* ✅ Turing Machines
* ✅ Computational models
* ✅ Formal language theory

---

# 🧪 How to Use

### 1️⃣ Clone the Repository

```bash
git clone <your-repository-url>
```

### 2️⃣ Navigate to the Repository

```bash
cd Theory-of-Automata-Practicals
```

### 3️⃣ Install Python

Make sure Python is installed on your system.

### 4️⃣ Open the Notebooks

Open the `code` directory using **Jupyter Notebook**, **JupyterLab**, or **VS Code**.

For example:

```bash
jupyter notebook
```

### 5️⃣ Run the Notebooks

Start with:

```text
01_nfa_to_dfa.ipynb
```

and progress through the notebooks in numerical order.

---

# 📌 Repository Purpose

This repository is primarily an **academic and learning resource** created while studying **Theory of Automata / Theory of Computation** at university.

It brings together practical implementations and supporting course material in one place, making it useful for:

* 📖 Course revision
* 🧪 Practical preparation
* 💻 Algorithm implementation
* 🎓 University assignments
* 🔄 Reviewing automata concepts
* 🧠 Understanding computational models

---

## 🏷️ Topics

<p align="center">

![Automata](https://img.shields.io/badge/Automata-Theory-8A2BE2?style=flat-square)
![NFA](https://img.shields.io/badge/NFA-Automata-blue?style=flat-square)
![DFA](https://img.shields.io/badge/DFA-Automata-2E8B57?style=flat-square)
![Minimization](https://img.shields.io/badge/DFA-Minimization-orange?style=flat-square)
![Formal Languages](https://img.shields.io/badge/Formal-Languages-red?style=flat-square)
![PDA](https://img.shields.io/badge/Pushdown-Automata-purple?style=flat-square)
![Turing Machines](https://img.shields.io/badge/Turing-Machines-black?style=flat-square)
![CNF](https://img.shields.io/badge/Chomsky-Normal%20Form-yellow?style=flat-square)

</p>

---

## 👨‍💻 Author

**Muhammad Ali**

[![GitHub](https://img.shields.io/badge/GitHub-AliMuhammad78-181717?style=flat-square\&logo=github\&logoColor=white)](https://github.com/AliMuhammad78)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Muhammad%20Ali-0A66C2?style=flat-square\&logo=linkedin\&logoColor=white)](https://www.linkedin.com/in/muhammad-ali-91294a290)
[![Kaggle](https://img.shields.io/badge/Kaggle-ali98muhammad45-20BEFF?style=flat-square\&logo=kaggle\&logoColor=white)](https://www.kaggle.com/ali98muhammad45)

---

<p align="center">

⭐ <strong>Theory of Automata — From Finite Automata to Turing Machines</strong>

</p>
