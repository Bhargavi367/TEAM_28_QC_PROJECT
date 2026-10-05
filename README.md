# QSchedule

<p align="center">
  <img src="logo.png" width="110" alt="QSchedule Logo">
</p>

<p align="center">
  <b>Quantum-Optimized Hospital Appointment Scheduling</b>
</p>

<p align="center">
  <i>“Don’t just find an available slot. Find the smarter one.”</i>
</p>

---

## About QSchedule

**QSchedule** is a quantum-optimized hospital appointment scheduling system designed to make complex hospital scheduling more efficient.

In a hospital, scheduling is not simply about finding an empty time slot. A single appointment may depend on the availability of a doctor, room, medical resources, patient priority, appointment duration, and existing bookings.

When these constraints increase, finding an efficient schedule becomes a **combinatorial optimization problem**.

QSchedule explores the use of **quantum optimization techniques** to find better scheduling combinations while respecting important hospital constraints.

---

## Why QSchedule?

Traditional appointment systems mainly answer:

> **“Is this slot available?”**

QSchedule focuses on:

> **“Which available slot creates the best overall schedule?”**

This makes QSchedule different from a basic appointment-booking system. Instead of treating every appointment independently, it considers the **overall hospital scheduling environment**.

---

## Key Objectives

* Reduce patient waiting time.
* Avoid doctor scheduling conflicts.
* Improve room utilization.
* Balance doctor workloads.
* Consider patient priority.
* Handle multiple scheduling constraints.
* Explore quantum optimization for healthcare.
* Generate an efficient and feasible appointment schedule.

---

## Quantum Approach

QSchedule models hospital appointment scheduling as an optimization problem.

The problem can be represented using a **QUBO (Quadratic Unconstrained Binary Optimization)** formulation, where scheduling decisions are represented through binary variables.

The optimization objective can consider:

```text
Scheduling Cost
      =
Patient Waiting Time
+ Doctor Idle Time
+ Resource Conflicts
+ Constraint Penalties
```

The project explores **QAOA (Quantum Approximate Optimization Algorithm)** as a possible quantum approach for solving the optimization problem.

A hybrid quantum-classical approach can also be used, where classical computing prepares and validates the data while quantum optimization handles the complex search space.

---

## Main Components

### Patient Management

Stores appointment information such as patient details, required specialization, preferred time, priority, and appointment duration.

### Doctor Management

Maintains doctor specialization, availability, working hours, existing appointments, and workload.

### Resource Management

Handles consultation rooms, diagnostic rooms, equipment, and other scheduling resources.

### Optimization Engine

Converts scheduling requirements into an optimization model and searches for a high-quality feasible schedule.

### Appointment Scheduler

Uses the optimized result to assign patients to suitable doctors, rooms, and time slots.

---

## Simple Architecture

```text
Patient + Doctor + Room Data
            ↓
     Scheduling Model
            ↓
      QUBO Formulation
            ↓
   Quantum / Hybrid Solver
            ↓
   Feasibility Validation
            ↓
      Final Schedule
```

---

## Example

A generated schedule may look like:

| Patient | Doctor | Room | Time  | Priority |
| ------- | ------ | ---- | ----- | -------- |
| P001    | Dr. A  | R01  | 09:00 | High     |
| P002    | Dr. B  | R02  | 09:30 | Normal   |
| P003    | Dr. A  | R01  | 10:00 | Normal   |

The final schedule depends on the input data and optimization constraints.

---

## Technology Stack

**Programming:** Python

**Quantum Computing:** Qiskit, QAOA, Quantum Simulator

**Optimization:** QUBO, Classical Optimization

**Data Processing:** NumPy, Pandas

**Frontend:** HTML, CSS, JavaScript *(if implemented)*

**Backend:** Flask / FastAPI *(if implemented)*

**Database:** SQLite / MySQL *(if implemented)*

---

## What Makes QSchedule Unique?

QSchedule does not treat hospital appointment booking as a simple **first-come, first-served slot selection problem**.

It treats the hospital as a connected system where:

**Patient + Doctor + Room + Time + Priority = One Optimization Problem**

A change in one appointment can affect several other appointments.

QSchedule aims to find a scheduling arrangement where these relationships are considered together rather than separately.

---

## Expected Benefits

### For Patients

* Lower waiting time
* Better appointment allocation
* Improved priority handling
* Fewer scheduling conflicts

### For Doctors

* Better workload distribution
* Organized schedules
* Reduced idle periods

### For Hospitals

* Improved room utilization
* Better resource allocation
* More efficient scheduling
* Reduced scheduling complexity

---

## Future Scope

QSchedule can be expanded into a larger hospital optimization platform.

Future possibilities include:

* AI-based appointment duration prediction
* Emergency-aware dynamic scheduling
* Multi-hospital appointment optimization
* Real-time resource allocation
* Mobile application for patients
* AI + Quantum hybrid optimization
* Operation theatre scheduling
* Diagnostic laboratory scheduling
* Staff scheduling
* ICU resource optimization

---

## Project Vision

> **A hospital should not simply ask what is available. It should determine what is optimal.**

QSchedule explores how quantum optimization can be applied to a practical healthcare problem and how complex scheduling decisions can be transformed into an intelligent optimization process.

The ultimate vision is simple:

**Smarter schedules → Better resource utilization → Better patient experience.**

---

## Team

| Name                 | Roll Number    |
| -------------------- | -------------- |
| **K. Sai Vaishnavi** | **2420030660** |
| **K. Bhargavi**      | **2420030661** |

---

## QSchedule

### *Quantum Intelligence. Smarter Scheduling. Better Healthcare.*
