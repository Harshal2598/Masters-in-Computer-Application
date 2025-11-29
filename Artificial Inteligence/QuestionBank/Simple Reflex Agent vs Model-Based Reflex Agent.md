# 🤖 Simple Reflex Agent vs Model-Based Reflex Agent

AI agents behave differently depending on how much information they use to make decisions.  
Two important types are **Simple Reflex Agents** and **Model-Based Reflex Agents**.

---

# 🆚 Difference Between Simple Reflex Agent and Model-Based Reflex Agent

| Feature | Simple Reflex Agent | Model-Based Reflex Agent |
|--------|----------------------|---------------------------|
| **Definition** | Acts only based on the *current percept*. | Acts based on *current percept + internal model* of the world. |
| **Memory** | No memory; does not store past information. | Has memory; stores and updates past information. |
| **Environment Type** | Works only in **fully observable** environments. | Works in **partially observable** environments. |
| **Complexity** | Simple and fast. | More complex and intelligent. |
| **Decision Basis** | Uses *condition-action rules* (IF-THEN). | Uses rules + internal state of the world. |
| **Limitations** | Cannot handle hidden or missing information. | Can handle incomplete or noisy information. |
| **Adaptability** | Low adaptability. | High adaptability. |
| **Example** | Vacuum cleans if it sees dirt now. | Vacuum remembers which rooms are already cleaned. |

---

# 🧠 Simple Reflex Agent (Explanation)

A **Simple Reflex Agent** makes decisions only using the **current percept**, without considering the past.

### ✔ How it works:
IF condition THEN action


### ✔ Example:
A vacuum cleaner:
- If it senses **dirty** → CLEAN  
- If it senses **clean** → MOVE  

It does NOT remember which room it cleaned earlier.

---

# 🧠 Model-Based Reflex Agent (Explanation)

A **Model-Based Reflex Agent** maintains an **internal model** (memory) of the environment.  
It uses past percepts + current percept to make better decisions.

### ✔ How it works:


Internal model + Current percept → Action


### ✔ Example:
A smart vacuum cleaner:
- Remembers which rooms were cleaned  
- Knows obstacles even if sensors don’t detect them now  
- Decides next move based on stored knowledge  

It works well in **partially observable** environments.

---

# 📝 Short Exam Answer

- A **Simple Reflex Agent** responds only to the current percept using condition–action rules. It works in fully observable environments. Example: A vacuum cleaner that cleans only when it sees dirt.
  
- A **Model-Based Reflex Agent** uses the current percept plus an internal model (memory) to handle partia
