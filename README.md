# 📅 Day 5 – Flip-Flops in Digital Electronics

## 📌 What I Learned

### 🔁 What Are Flip-Flops?

Flip-flops are basic memory elements in digital electronics that store 1-bit of data. They change state only on the edge of a clock signal.

---

## 📘 Types of Flip-Flops

### 1️⃣ D (Data) Flip-Flop

**Rule:**  
On clock edge, Q = D

**Truth Table:**

| Clock | D | Q (Next) |
|-------|---|----------|
| ↑     | 0 | 0        |
| ↑     | 1 | 1        |

**Use Case:** Registers, memory units

---

### 2️⃣ SR (Set-Reset) Flip-Flop

**Rules:**  
- S=1, R=0 → Q = 1 (Set)  
- S=0, R=1 → Q = 0 (Reset)  
- S=0, R=0 → Hold  
- S=1, R=1 → Invalid

**Truth Table:**

| S | R | Q (Next) |
|---|---|----------|
| 0 | 0 | Hold     |
| 1 | 0 | 1        |
| 0 | 1 | 0        |
| 1 | 1 | ❌ Invalid |

**Use Case:** Simple control logic

---

### 3️⃣ T (Toggle) Flip-Flop

**Rule:**  
- T = 0 → Hold  
- T = 1 → Toggle Q

**Truth Table:**

| T | Q (Prev) | Q (Next) |
|---|----------|----------|
| 0 | 0        | 0        |
| 0 | 1        | 1        |
| 1 | 0        | 1        |
| 1 | 1        | 0        |

**Use Case:** Counters, clocks

---

### 4️⃣ JK Flip-Flop (Universal Flip-Flop)

**Rule:**  
- J=0, K=0 → Hold  
- J=1, K=0 → Set  
- J=0, K=1 → Reset  
- J=1, K=1 → Toggle

**Truth Table:**

| J | K | Q (Next) |
|---|---|----------|
| 0 | 0 | Hold     |
| 1 | 0 | 1        |
| 0 | 1 | 0        |
| 1 | 1 | Toggle   |

**Use Case:** Versatile control circuits

---

## 🔂 Sequence Simulation (T Flip-Flop Example)

Start Q = 0, Input = 1 → 0 → 1 → 1

| Clock | T | Action   | Q |
|-------|---|----------|---|
| 1     | 1 | Toggle   | 1 |
| 2     | 0 | Hold     | 1 |
| 3     | 1 | Toggle   | 0 |
| 4     | 1 | Toggle   | 1 |

✅ Final Q = 1

---

## 🔎 Flip-Flop Use Cases

| Flip-Flop | Used In                        |
|-----------|-------------------------------|
| D         | Registers, memory             |
| SR        | Set/reset control             |
| T         | Frequency dividers, counters  |
| JK        | Complex sequential logic      |

---

## 🎯 Quiz Results

| Quiz        | Score |
|-------------|-------|
| Flip-Flop 1 | 4/8   |
| Flip-Flop 2 | 6/8   |

🟢 Strong in: T, D Flip-Flop  
🔴 Need to revise: SR invalid state, JK toggle

---

## 🔗 GitHub Reflection

> Flip-flops form the core of VLSI logic circuits. Understanding their clock-based behavior and output transitions prepares me for designing memory, counters, and processors.

---

### #VLSI #DigitalDesign #SequentialCircuits #FlipFlop #Day5
