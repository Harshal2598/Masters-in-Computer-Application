# 🌍 Environment in Artificial Intelligence (AI)

## **What is an Environment in AI?**

In Artificial Intelligence, an **environment** is everything that surrounds an agent and interacts with it.  
It provides **input** to the agent and receives **output actions** from the agent.

In simple terms:

> **Environment = The external world in which an AI agent operates and makes decisions.**

Examples of environment:
- A chess board (for a chess-playing AI)
- A road (for a self-driving car)
- A house (for a cleaning robot)
- Stock market (for a trading AI)

The agent **perceives** the environment through sensors and **acts** on it using actuators.

---

# ⭐ Features of an AI Environment (Explained in Detail)

AI environments have several important characteristics. Each characteristic affects how difficult or easy it is for an AI agent to perform tasks.

---

## **1. Fully Observable vs Partially Observable**
- **Fully Observable:**  
  The agent has complete information about the environment.  
  **Example:** Chess game – all pieces are visible.
  
- **Partially Observable:**  
  The agent does not have full information.  
  **Example:** Self-driving car in fog; it can’t see everything.

---

## **2. Deterministic vs Stochastic**
- **Deterministic:**  
  The next state is completely predictable from the current state and action.  
  **Example:** Calculator operations.

- **Stochastic:**  
  The next state is uncertain and involves randomness.  
  **Example:** Weather prediction, stock market.

---

## **3. Episodic vs Sequential**
- **Episodic:**  
  Each task (episode) is independent of previous tasks.  
  **Example:** Image classification – each image is separate.

- **Sequential:**  
  Current decisions affect future outcomes.  
  **Example:** Self-driving car – previous moves matter.

---

## **4. Static vs Dynamic**
- **Static:**  
  Environment does not change during the agent’s thinking.  
  **Example:** Crossword puzzles.

- **Dynamic:**  
  Environment keeps changing during decision-making.  
  **Example:** Traffic while driving.

---

## **5. Discrete vs Continuous**
- **Discrete:**  
  Limited number of actions or states.  
  **Example:** Chess – limited moves.

- **Continuous:**  
  Infinite states or actions.  
  **Example:** Robot arm movements, real-world driving.

---

## **6. Single Agent vs Multi-Agent**
- **Single Agent:**  
  Only one agent acts in the environment.  
  **Example:** A cleaning robot.

- **Multi-Agent:**  
  Multiple agents interact or compete.  
  **Example:** Online multiplayer gaming, stock market trading.

---

## **7. Known vs Unknown**
- **Known Environment:**  
  All rules and outcomes are known to the agent.  
  **Example:** Board games like Tic-Tac-Toe.

- **Unknown Environment:**  
  The agent must learn the rules by interacting with the environment.  
  **Example:** Real-life problems like market prediction.

---



