# 🤖 Goal-Based Agents and Utility-Based Agents

AI agents vary in intelligence depending on how they make decisions.  
Two important types are **Goal-Based Agents** and **Utility-Based Agents**.

---

# 🎯 1. What is a Goal-Based Agent?

A **Goal-Based Agent** is an AI agent that chooses actions based on achieving a **specific goal**.  
It does not just react; it **thinks about future consequences** and selects actions that move it closer to its goal.

### ✔ Key Features:
- Uses a **goal** to guide decisions.
- Performs **search** or **planning** to choose the best action.
- Considers the **future outcome** before acting.
- More intelligent than reflex agents.

---

## 🧠 How Goal-Based Agents Work (Step-by-Step)

1. **Perceive the environment** (sensor input).  
2. **Compare current state** with the **goal state**.  
3. **Plan** a sequence of actions.  
4. **Choose the action** that moves closer to the goal.  
5. **Execute action** and repeat until goal is achieved.

---

## 🌍 Real-Life Examples of Goal-Based Agents

### 🛣 Example 1: GPS Navigation System
- **Goal:** Reach destination.
- Perceives position using GPS.
- Calculates shortest route.
- Chooses actions: turn left, go straight, etc.
- Updates route if traffic changes.

### 🧹 Example 2: Smart Vacuum Cleaner (Advanced)
- **Goal:** Clean the entire room.
- Maps rooms and plans cleaning path.
- Goes to unclean areas until the goal is complete.

### 🤖 Example 3: Self-Driving Car
- **Goal:** Reach destination safely.
- Plans overtaking, stopping, speed control based on future outcomes.

---

# 📌 Short Definition for Exams
A **Goal-Based Agent** selects actions by considering goals and planning future steps to achieve them.

---

# 💡 2. What is a Utility-Based Agent?

A **Utility-Based Agent** not only aims for a goal but also tries to achieve the **best possible outcome**.

It measures happiness, usefulness, or satisfaction using a **utility function**.

### ✔ Key Features:
- Has **goals + preferences**.
- Calculates **utility** (score) for every possible action.
- Chooses the action with the **highest utility value**.
- Works well in uncertain or complex environments.

---

## 🧮 Simple Utility Function Example

Utility = Happiness, Profit, Comfort, Safety, Speed, etc.

---

## 🍔 Example: Choosing Food Delivery

A utility-based agent calculates utility:

| Option | Taste Score | Price | Delivery Time | Utility |
|--------|-------------|-------|----------------|---------|
| Pizza  | 9/10        | High  | Fast           | 7.5     |
| Burger | 7/10        | Low   | Medium         | 7.0     |
| Salad  | 5/10        | Low   | Fast           | 6.0     |

**Utility-Based Agent chooses Pizza** because it gives the **highest overall utility**, not just the cheapest or fastest.

---

## 🚗 Example: Self-Driving Car (Utility-Based)

- Goal-based car: reach destination.  
- Utility-based car: reach destination **safely, quickly, comfortably**.

It evaluates:
- Safety score  
- Fuel use  
- Comfort  
- Travel time  

And picks the best action.

---

# 📝 Short Exam Answer

- A **Goal-Based Agent** chooses actions by planning and selecting steps that achieve a desired goal. Example: A GPS navigation system plans the shortest route to the destination.

- A **Utility-Based Agent** selects actions based on which one provides the **highest utility (benefit)**. Example: A food delivery AI choosing the meal with the best combination of taste, price, and delivery time.

