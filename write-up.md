# Daily Reflection Tree — Design Rationale

## 1. Introduction

This project is a deterministic, decision-tree-based reflection tool designed to help individuals reflect on their day in a structured and meaningful way.
The system avoids free-text input and instead uses predefined options, ensuring that every interaction is consistent, predictable, and auditable.

The goal of this tool is not to judge the user, but to guide them toward self-awareness through carefully designed questions and reflections.

---

## 2. Psychological Framework

The tree is built around three core psychological dimensions:

### Axis 1 — Locus of Control

This axis explores whether the user interprets events as something that happened *to them* (external locus) or something they had influence over (internal locus).
It is inspired by Rotter’s Locus of Control theory and Dweck’s Growth Mindset.

### Axis 2 — Contribution vs Entitlement

This axis evaluates whether the user focuses more on what they *gave* versus what they *expected or deserved*.
It is based on concepts like Organizational Citizenship Behavior and Psychological Entitlement.

### Axis 3 — Radius of Concern

This axis expands the user’s perspective from self → team → others → end user.
It is inspired by Maslow’s concept of self-transcendence and perspective-taking theory.

---

## 3. Design Principles

* **Deterministic Flow:** Every user choice leads to a predefined next node. No randomness is used.
* **No Free Text:** All inputs are fixed options to ensure consistency and clarity.
* **Progressive Depth:** Each axis starts with a broad question and then deepens through follow-up questions.
* **Non-Judgmental Tone:** Reflections are designed to guide awareness, not assign blame.
* **Actionable Insight:** Each reflection encourages a small shift in thinking or behavior.

---

## 4. Tree Structure

The reflection flow follows a fixed sequence:

**Axis 1 (Locus) → Axis 2 (Contribution) → Axis 3 (Radius) → Summary → End**

Each axis contains:

* One initial question (broad reflection)
* One follow-up question (deeper insight)
* Multiple reflection nodes based on user choices

This creates a structured yet personalized reflection journey.

---

## 5. Branching Logic

The system operates entirely on deterministic branching:

* Each option maps to a specific next node.
* Decision nodes assign signals such as:

  * `axis1:internal` or `axis1:external`
  * `axis2:contribution` or `axis2:entitlement`
  * `axis3:self`, `axis3:team`, `axis3:beyond`
* No machine learning or LLM is used at runtime.
* Given the same inputs, the system will always produce the same output.

---

## 6. Reflection Design

Reflections are carefully written to:

* Reinforce awareness without judgment
* Highlight patterns in thinking
* Encourage small behavioral shifts
* Maintain a conversational and human tone

Each reflection is tied to a specific branch of the tree, ensuring relevance to the user's choices.

---

## 7. Limitations and Improvements

While the current system is effective, it can be improved further:

* Add dynamic summary generation using collected signals
* Increase depth with additional follow-up questions
* Expand signal tracking for better pattern analysis
* Introduce visualization of user trends over time

---

## 8. Conclusion

This project demonstrates how psychological frameworks can be translated into a structured, deterministic system.
Instead of relying on AI-generated responses, the intelligence is embedded in the design of the tree itself.

The result is a predictable, scalable, and user-friendly reflection tool that encourages deeper thinking and continuous self-improvement.
