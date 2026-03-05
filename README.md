# Verilog Washing Machine Controller using Finite State Machine (FSM) in Verilog

## 📌 Project Overview

This project implements an **Automatic Washing Machine Controller** using a **Finite State Machine (FSM)** in **Verilog HDL**.
The controller manages different stages of the washing process such as:

* Checking the door status
* Filling water
* Adding detergent
* Washing cycle
* Draining water
* Spinning clothes

The design simulates how a real washing machine automatically transitions between different stages based on sensor inputs and timing signals.



## ⚙️ Features

* FSM based control system
* Sequential logic design using Verilog
* Automatic stage transitions
* Simulation compatible with **Xilinx Vivado**
* Clear modular structure



## 🧠 FSM States

The washing machine controller consists of the following states:

| State           | Description                                    |
| --------------- | ---------------------------------------------- |
| `CHECK_DOOR`    | Verifies if the door is closed before starting |
| `FILL_WATER`    | Water is filled into the machine               |
| `ADD_DETERGENT` | Detergent is added for washing                 |
| `CYCLE`         | Washing operation is performed                 |
| `DRAIN_WATER`   | Used water is drained                          |
| `SPIN`          | Final spinning to remove excess water          |



## 📥 Inputs

| Input             | Description                      |
| ----------------- | -------------------------------- |
| `clk`             | System clock                     |
| `reset`           | Reset signal                     |
| `door_close`      | Indicates whether door is closed |
| `start`           | Starts the washing process       |
| `filled`          | Water level sensor               |
| `detergent_added` | Indicates detergent is added     |
| `cycle_timeout`   | Washing cycle completion signal  |
| `drained`         | Water drain completion           |
| `spin_timeout`    | Spin cycle completion            |



## 📤 Outputs

| Output          | Description                          |
| --------------- | ------------------------------------ |
| `doorlock`      | Locks washing machine door           |
| `motor_on`      | Controls washing motor               |
| `fillvalue_on`  | Activates water inlet valve          |
| `drainvalue_on` | Activates drain valve                |
| `done`          | Indicates washing process completion |
| `soapwash`      | Soap wash stage indicator            |
| `waterwash`     | Water wash stage indicator           |



## 🔄 Working Principle

1. The system starts in **CHECK_DOOR** state.
2. If the **door is closed** and **start is pressed**, the machine begins operation.
3. Water is filled in the **FILL_WATER** state.
4. Detergent is added in **ADD_DETERGENT** state.
5. The **CYCLE** state performs the washing process.
6. Used water is removed in **DRAIN_WATER** state.
7. The **SPIN** state performs the final drying process.
8. After spinning completes, the system signals **DONE**.






## 🛠 Tools Used

* **Verilog HDL**
* **Xilinx Vivado**
* **Digital Logic Design**
* **Finite State Machine (FSM)**



## ▶️ Simulation

The design can be simulated using **Vivado Simulator** .

Steps:

1. Create a new Vivado project
2. Add the Verilog source file
3. Add the testbench file
4. Run behavioral simulation



## 📚 Applications

* Embedded control systems
* Digital appliance controllers
* FSM based automation systems
* Educational digital design projects



## 👩‍💻 Author

Mamatha Kodari/ECE/Verilog-washing-machine
