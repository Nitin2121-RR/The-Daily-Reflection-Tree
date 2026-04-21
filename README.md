# Daily Reflection Tree

A deterministic, decision-tree-based reflection system designed to guide users through structured end-of-day self-reflection.

---

## 🚀 What is this?

This project implements a **deterministic reflection tree** that helps users analyze their day through a sequence of structured questions and reflections.

The system is based on three psychological dimensions:

* **Axis 1 — Locus of Control (Victim ↔ Victor)**
* **Axis 2 — Contribution vs Entitlement**
* **Axis 3 — Radius of Concern (Self ↔ Others ↔ Beyond)**

The goal is to help users gain clarity about their mindset and actions — not through AI-generated responses, but through a carefully designed tree.

---

## ⚙️ How it Works

1. The user starts at the **START node**
2. Each node presents a **fixed set of options**
3. Based on the selected option, the system moves to the next node
4. The flow continues across all three axes
5. The session ends with a **summary reflection**

👉 The system is fully deterministic:

* Same input → Same path → Same output

---

## 🌳 Project Structure

```text id="g0v0g8"
/tree/
  reflection-tree.json     # Core decision tree logic
  tree-diagram.png         # Visual representation of the tree

write-up.md                # Explanation of design decisions
README.md                  # Project overview
```

---

## 📊 Tree Design Overview

* **Total Nodes:** 30+
* **Questions:** Multiple per axis
* **Decision Nodes:** Used for deterministic branching
* **Reflection Nodes:** Provide insights based on user choices
* **Bridges:** Connect axes smoothly
* **Summary:** Final reflection

Flow of the system:

```id="8xg8x6"
Axis 1 → Axis 2 → Axis 3 → Summary → End
```

---

## 🧠 Key Features

* ✅ Fully deterministic (no randomness)
* ✅ No free-text input
* ✅ No LLM or AI at runtime
* ✅ Structured decision-tree logic
* ✅ Psychology-driven design
* ✅ Consistent and auditable behavior

---

## 📌 Important Note

This project focuses on the **design of the reflection tree**, not on building a user interface.

* No web app or UI is implemented
* No runtime execution environment is required
* The tree itself is the core deliverable

The system can be executed by any external agent capable of reading the JSON structure.

---

## 💡 Future Improvements

* Build a CLI or web-based interface for interaction
* Add dynamic summaries using accumulated signals
* Track reflections over multiple days
* Visualize user behavior patterns over time

---

## 👨‍💻 Author

Developed as part of the **DT Fellowship Assignment**, focusing on knowledge engineering and deterministic system design.

---

## ⭐ Final Thought

> The intelligence of the system lies in the structure —
> not in generated responses.

---
