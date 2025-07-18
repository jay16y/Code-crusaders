# Entry Queue Management System

This C++ project simulates an intelligent queue management system for events with multiple entry gates. It aims to reduce waiting times and balance the load across all gates.

## 🔧 Key Features

- Random assignment of attendees to gates  
- Waiting time calculation per gate  
- Suggestion of the optimal (least busy) gate  
- Internal load balancing  
- Dedicated VIP gate handling  
- Group seating allocation

## 🧠 Core Logic

- Attendees are randomly assigned to gates.
- Waiting time is calculated as:  
  `waiting_time[i] = queue_size[i] * P`
- The gate(s) with minimum waiting time are suggested to new entrants.
- Gates are rebalanced internally for even queue distribution.
- VIPs and groups are handled with custom logic.

## 📂 Functions

- `random_assignment()`
- `Calculate_waiting_time()`
- `suggest_queue()`
- `internal_assignment()`
- `random_assignment_of_VIP()`
- `group_system()`
