# 🔍 Fully Observable vs Partially Observable Environments (AI)

In Artificial Intelligence, an environment may or may not provide complete information to the agent.  
Based on the availability of information, environments are classified into **fully observable** and **partially observable**.

---

## ✅ **Difference Between Fully Observable and Partially Observable Environments**

| Feature | Fully Observable Environment | Partially Observable Environment |
|--------|------------------------------|----------------------------------|
| **Definition** | The agent has complete and accurate information about the environment’s state. | The agent has incomplete, limited, or noisy information about the environment. |
| **Visibility** | All relevant data is visible to the agent. | Some data is hidden or uncertain. |
| **Decision Making** | Easier, because the agent knows everything it needs. | Difficult, because the agent must guess or predict missing information. |
| **Complexity** | Low complexity. | High complexity. |
| **Use of Memory** | Memory not required to store past states. | Memory is needed to remember past events. |
| **Sensors** | Perfect sensors. | Imperfect or limited sensors. |

---

## 🧠 **Examples**

### **1. Fully Observable Environment**
- **Chess game**  
  → The agent can see the entire board: all pieces and their positions.  
- **Tic-Tac-Toe**  
  → Every cell is visible to both players.  
- **Sudoku**  
  → All given numbers are visible and fixed.

### **2. Partially Observable Environment**
- **Self-driving car in traffic**  
  → Can’t see behind buildings, around corners, or in fog.  
- **Poker or card games**  
  → Other players’ cards are hidden.  
- **Medical diagnosis**  
  → Doctor (agent) cannot see internal symptoms directly.

---



