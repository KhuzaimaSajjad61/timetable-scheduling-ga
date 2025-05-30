# Timetable Scheduler using Genetic Algorithm 🧬

This project implements a Genetic Algorithm (GA) to solve the class timetable scheduling problem. It efficiently assigns courses to time slots, professors, sections, and classrooms, while respecting both hard and soft constraints.

## 📖 Overview

The scheduling problem is modeled as a genetic optimization problem where:

- Each **chromosome** represents a full timetable.
- Each **gene** represents the assignment of a course to a section, professor, rooms, and time slots.
- A **fitness function** evaluates how well the solution satisfies constraints.
- **Selection, crossover, and mutation** operators evolve better solutions over generations.

The algorithm continues evolving the population until an optimal or near-optimal timetable is found.

## 🎯 Features

- Enforces hard constraints:
  - Professors/sections/rooms cannot be double-booked
  - Max course limits per professor and section
  - Room size must accommodate section strength
- Rewards soft preferences:
  - Morning theory classes and afternoon labs
  - Same room usage for a course
  - Continuous teaching blocks
  - Minimized movement between floors

## ▶️ How to Run

1. **Clone the repository**:

   ```bash
   git clone https://github.com/KhuzaimaSajjad61/timetable-scheduler-ga.git
   cd timetable-scheduler-ga

2. **Install dependencies**:
   
   ```bash
   pip install -r requirements.txt

3. **Launch the notebook**:
   
   ```bash 
   jupyter notebook scheduler.ipynb
