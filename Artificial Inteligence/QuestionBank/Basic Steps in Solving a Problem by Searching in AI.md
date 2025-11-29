# 🔍 Basic Steps in Solving a Problem by Searching in AI

In Artificial Intelligence, **search** is used to find a sequence of actions that lead from the **initial state** to the **goal state**.  
Every search algorithm follows a set of common steps.

Below are the **basic steps in solving a problem by searching**:

---

## 1️⃣ **Define the Problem**
The first step is to clearly define the components of the problem:
- **Initial State:** The starting point  
- **Goal State:** The desired result  
- **Actions/Operators:** What actions can be taken  
- **Path Cost:** Cost of each action  

Example:  
In a route-finding problem → start city, destination city, and available roads.

---

## 2️⃣ **Formulate the Problem as a State Space**
A **state space** is a representation of all possible states and actions.

- Each state = a situation  
- Each action = transition to a new state  

Example:  
Chess → Each board configuration is a state.

---

## 3️⃣ **Choose a Search Strategy**
The agent must decide **how** to explore the state space.

Strategies include:
- **Uninformed Search:** BFS, DFS, UCS  
- **Informed Search:** Greedy, A*, Hill Climbing  

The choice depends on time, space, and problem complexity.

---

## 4️⃣ **Initialize the Search Tree**
- Start by creating a **node** for the initial state.
- Add it to the **frontier** (open list).

The frontier is the set of nodes waiting to be explored.

---

## 5️⃣ **Expand Nodes**
Repeat the following steps:
1. Remove a node from the frontier  
2. Check if it is the **goal state**  
3. If not, **expand** it  
4. Generate all successor states  
5. Add them to the frontier  

This process continues until the goal is found or frontier becomes empty.

---

## 6️⃣ **Goal Test**
At each node:
- Compare current state with the **goal state**  
- If it matches → solution found  

Example:  
In a maze, if agent reaches the exit, search stops.

---

## 7️⃣ **Construct the Solution (Backtracking)**
Once the goal node is found:
- Trace back from the goal to the initial state  
- Collect the sequence of actions  

This becomes the **solution path**.

Example:  
Shortest route shown in Google Maps.

---

# 📝 Short Exam Answer

The basic steps in solving a problem by searching are:
1. **Define the problem** (initial state, goal state, actions, path cost).  
2. **Formulate the state space** representing all possible states.  
3. **Select a search strategy** (BFS, DFS, A*, etc.).  
4. **Initialize the search tree** with the initial node.  
5. **Expand nodes** by generating successors.  
6. **Apply goal test** to check if the goal is reached.  
7. **Construct the solution** by tracing back the path from goal to start.

These steps allow an AI agent to systematically explore the environment and find the best solution.

