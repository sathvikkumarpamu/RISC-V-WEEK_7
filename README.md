# 🚀 BabySoC Physical Design – Week 7  
### **Complete RTL → Layout Flow Using OpenROAD (Floorplan • Placement • Routing • SPEF)**

This repository documents the complete physical-design flow for **BabySoC** using the **OpenROAD** toolchain.  
It covers all backend stages—from floorplanning to post-route parasitic extraction (SPEF).

---

## 📘 **Objective**
To perform the full physical-design implementation of the *BabySoC* SoC block using OpenROAD, including:

- ✔ Floorplanning  
- ✔ Placement  
- ✔ Routing  
- ✔ Post-route SPEF generation  

and to understand how these stages integrate into a real SoC backend flow.

---

## 🧠 **Why This Task Matters**
Until this point, each VLSI stage (RTL, SPICE, synthesis, early floorplanning) was explored separately.  
This week, all stages are combined into a **complete RTL-to-layout flow**, giving real-world SoC design experience.

### 🎯 **Key Learning Outcomes**
By completing this task, you will:

- 🔹 Understand how a **full RTL-to-GDS backend flow** works  
- 🔹 Learn how **floorplan choices**, **placement density**, and **routing topology** affect timing  
- 🔹 Perform **post-route parasitic extraction (SPEF)**  
- 🔹 Understand how SPEF feeds into **Static Timing Analysis (STA)**  
- 🔹 Bridge the gap between theory (STA) and real SoC physical design  

This is an essential foundation for anyone aiming to become a **professional ASIC Physical Design Engineer**.

---

## 📚 **Task Reference**
The flow follows **Task 13 – OpenROAD Physical Design** from:

🔗 **Akash-Perla / ASIC-Design Repository**  
https://github.com/Akash-Perla/ASIC-Design?tab=readme-ov-file#task-13-OpenRoad-Physical-Design

---

# 🧩 Physical Design Flow Summary

## 1️⃣ **Floorplanning**
- Import synthesized BabySoC netlist  
- Define die area, core area & utilization  
- Create **power rings & straps**  
- Place macros and reserve cell placement regions  
- Ensure a clean and routable floorplan  

---

## 2️⃣ **Placement**
- Run **global placement**  
- Perform **detailed placement + legalization**  
- Check placement density & congestion  
- Export placement layout snapshots  

---

## 3️⃣ **Routing**
- Execute **global routing**  
- Run **detailed routing**  
- Verify **zero routing DRC violations**  
- Save final routed layout images  

---

## 4️⃣ **Post-Route SPEF Extraction**
- Extract parasitics using OpenROAD  
- Generate the **Standard Parasitic Exchange Format (SPEF)** file  
- Validate R & C values per net  
- Understand how SPEF improves STA timing accuracy  

---

# 📂 Deliverables in This Repository

### 📁 **layout_images/**
- Floorplan screenshots  
- Placement layout  
- Routed design  

### 📁 **logs/**
- SPEF generation terminal logs  
- Routing logs  
- Timing and congestion reports  

### 📁 **docs/**
- Commands used in the OpenROAD flow  
- Observations and learning notes  

### 📁 **reports/**
- Cell count  
- Utilization report  
- Number of routed nets  
- SPEF summary  

---

# 📝 Final Takeaways
By completing this task, you will have:

✔ Implemented a full physical-design flow for BabySoC using OpenROAD  
✔ Performed parasitic extraction and interpreted SPEF  
✔ Understood backend timing, routing, and congestion behavior  
✔ Connected STA theory to real ASIC layout implementation  
✔ Strengthened practical ASIC Design (PD) skills for career/industry  

---

## 📬 **Author**
BabySoC Week-7 Physical Design Task • OpenROAD Flow  
Feel free to contribute, fork, or ask questions!

---

