# Timetable Scheduling using Genetic Algorithm

## 📘 Project Overview

This project focuses on solving the **university timetable scheduling problem** using a **Genetic Algorithm (GA)**. Generating a conflict-free, efficient timetable is a complex task due to various hard and soft constraints involving professors, classrooms, time slots, and course requirements.

The aim of the project is to **automatically generate a valid timetable** that satisfies hard constraints (e.g., no double-booking, room capacity limits) and optimizes for soft constraints (e.g., teacher preferences, room consistency).


---

## 🧠 Key Features

- Efficient handling of **hard constraints**:
  - No professor or classroom double-booked
  - Proper room allocation according to section size
  - Theory and lab sessions scheduled appropriately

- Optimization of **soft constraints**:
  - Consistent room assignments
  - Minimizing idle periods for professors
  - Logical theory and lab time placements

---

## 🔧 Tools and Technologies

- **Python**: Core programming language
- **Libraries Used**:
  - `random`: Random number generation for crossover/mutation
  - `math`: Time-related calculations
  - `pandas`: Dataset manipulation and analysis
  - `collections.defaultdict`: Simplified data structure handling

---

## 🗃️ Dataset Information

The system uses **predefined datasets** including:

- **Courses**: Course ID, type (theory/lab), and weekly sessions
- **Professors**: Instructor list with teaching qualifications
- **Classrooms**: Room types and capacities

Each course receives either:
- Two theory lectures per week (with 15-minute gaps)
- One 3-hour lab session

---

## 🧬 Genetic Algorithm Structure

Each solution (chromosome) represents a possible timetable with:
- Course & type (theory/lab)
- Section and its size
- Assigned professor
- Room assignment
- Day/time slots

### Algorithm Phases:
1. **Population Initialization**: Generate initial random timetables
2. **Crossover**: Combine parent solutions to produce offspring
3. **Mutation**: Apply random modifications for diversity
4. **Fitness Evaluation**: Count and penalize conflicts
5. **Selection**: Choose best candidates for the next generation

---

## ✅ Results

- **Hard Constraints**: All met successfully
  - No double bookings or capacity violations
  - Correct room and time assignments
- **Soft Constraints**: Mostly satisfied
  - Lab/theory sessions scheduled in preferred time slots
  - Professors given continuous teaching blocks
  - Minimal room switching

---

## 📌 Conclusion

This project demonstrates how **genetic algorithms** can be applied to solve real-world **scheduling problems** efficiently. While the hard constraints were effectively managed, future improvements can focus on enhancing the fitness function to better satisfy soft constraints and adapt to real-time changes.

---

