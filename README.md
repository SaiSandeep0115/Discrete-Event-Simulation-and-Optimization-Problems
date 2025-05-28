# Discrete Event Simulation and Optimization Problems using Python Libraries

This repository presents two applied analytics projects that demonstrate the power of simulation and optimization in solving real-world operational challenges in service and supply chain domains.

---

## 🛠 Technologies & Libraries Used

- **Languages**: Python  
- **Libraries**:  
  - `SimPy` – Discrete Event Simulation  
  - `PuLP`, `Gurobi`, `OR-Tools` – Optimization (Mixed Integer Linear Programming)  
  - `Pandas`, `NumPy` – Data manipulation  
  - `Matplotlib`, `Seaborn` – Visualization  

---

## 📌 Project Overview

### 🔹 1. Discrete Event Simulation – Call Centre Performance

A simulated environment is created to model a call centre's operations over a full year (weekdays, 8 AM to 6 PM). The model evaluates key metrics such as:

- Call arrival rate
- Wait time
- Service time
- Percentage of calls answered within 1 minute (target = 90%)

**Objective**: Identify inefficiencies and provide data-driven recommendations for performance improvement.

#### 📊 Key Results

- **Total Calls Simulated**: 527  
- **% Answered Within 1 Minute**: 0.76%  
- **Average Wait Time**: 323.58 minutes (~5.4 hours)  
- **Average Service Time**: 4.95 minutes  

#### ⚠️ Implications & Recommendations

- **Issue**: Severely long wait times and low SLA compliance
- **Potential Causes**:
  - Understaffing
  - Ineffective call routing
  - Poor queue management

- **Recommended Actions**:
  - Increase staff or optimize scheduling
  - Implement self-service/automation
  - Improve workload distribution strategies

---

### 🔹 2. Linear Programming – Supply Chain Optimization

This section models the optimal production and distribution strategy for a company manufacturing 3 products and delivering to 2 regional warehouses.

#### 📦 Problem Scope

- **Maximize**: Total profit  
- **Constraints**:
  - Production capacity (hours)
  - Raw material limits (kg)
  - Warehouse demand & storage limits
  - Shipping & storage costs
  - Market balance (at least 40% shipped to Warehouse 1)

#### 📈 Optimization Outcome

- **Optimal Profit**: `$30,350.00`
- **Key Decisions**:
  - **Product A**: 200 units to Warehouse 1
  - **Product B**: Not produced
  - **Product C**: 250 units to Warehouse 1 & 250 units to Warehouse 2
- **Production time and material**: Fully utilized  
- **Market balance constraint**: Not binding

#### ✅ Tools Used

- **Solvers**: Gurobi, PuLP, OR-Tools  
- **Performance**: Solved in 5 iterations within 0.01 seconds  

---

## 📚 Educational Context

- Part 1 is designed for teaching Discrete Event Simulation in operations/service analytics.
- Part 2 demonstrates applied Mixed Integer Programming in supply chain contexts.
