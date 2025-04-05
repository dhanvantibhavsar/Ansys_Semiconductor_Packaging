<summary> <h2> From wafer to package: Assembly and Manufacturing Essentials </h2> </summary>
<details>
<summary> Setting The Stage - Supply Chain And Facilities </summary>

# 🧰 Semiconductor Packaging – Theory Overview

This section explains the **semiconductor supply chain** and provides a detailed look into a **package manufacturing unit** (ATMP – Assembly, Testing, Marking, and Packaging).

---

## 🔄 Semiconductor Supply Chain Overview

The semiconductor manufacturing supply chain is a multi-stage process that transforms raw silicon into fully functional end-user electronic products. Below are the key stages:

### 1. 🎨 **Design House**
- Inputs: EDA tools, Foundry PDKs
- Output: IC Design files (GDSII), Test programs
- Task: The chip is designed digitally using industry-standard EDA tools.

### 2. 🧪 **Wafer Fabrication**
- Inputs: Silicon wafers, Equipment, Gases, Chemicals, Materials
- Output: Wafer with fabricated ICs
- Task: Physical ICs are manufactured onto wafers using photolithography and other processes.

### 3. 📦 **Package Assembly and Test**
- Inputs: Substrates, Tools, Materials, Chemicals, Lids
- Output: Individual packaged ICs (e.g., Apple A15)
- Task: ICs are cut (diced), bonded, encapsulated, and tested. This is referred to as the ATMP process.

### 4. 🔧 **Board Assembly and Test**
- Inputs: PCBs, Tools, Materials
- Output: Assembled PCBs with IC packages
- Task: Multiple packaged ICs are mounted and tested on PCBs.

### 5. 📱 **Product Assembly and Test**
- Inputs: Components, Tools
- Output: Final consumer product (e.g., iPhone)
- Task: System-level integration and validation to produce the end product.

<img src="../images/module2/Screenshot 2025-04-05 164218.png" alt="Semiconductor Supply Chain Overview" width="600"/>

---

## 🏭 Introduction to a Package Manufacturing Unit (ATMP)

The **ATMP** process involves four core activities:  
**Assembly**, **Testing**, **Marking**, and **Packaging**.

### 🏢 Organization Type
- OSAT: Outsourced Semiconductor Assembly and Test providers  
  (e.g., ASE, Amkor, TATA)
- Alternatively, large companies (Intel, TSMC, Micron, Samsung) may run ATMP in-house.

### 🧰 Example Facility – Micron, Sanand (Gujarat)
- Total area: **1.4 million sq. ft.**
- Clean room area: **500,000 sq. ft.** (Class 1000/10000)
- Source: [Forbes India](https://www.forbesindia.com/)

### 🧱 Layout of an ATMP Unit

#### 🔹 Material Preparation and Storage
- Raw materials are staged for processing.

#### 🔹 Processing Zone
- Clean Room: ISO Class 6 & 7
- Key Steps:
  - Die bonding
  - Wire/Flip-chip bonding
  - Encapsulation
  - RDL (Redistribution Layer) formation

#### 🔹 Testing Area
- Electrical test
- Burn-in
- Reliability chamber testing

#### 🔹 Warehouse and Utility
- Storage of packaged ICs and system infrastructure

<img src="../images/module2/Screenshot 2025-04-05 164316.png" alt="Package Manufacturing Unit" width="600"/>

</details>

<details>
<summary> Wafer Pre-Preparation - Grinding And Dicing </summary>

# 🧪 Wafer Processing Inside the Cleanroom Area

This document outlines the sequence of steps involved in the wafer preparation process inside an **ISO Class 7 cleanroom**. The cleanroom environment is essential to maintain the cleanliness and integrity of semiconductor wafers during processing.

## 🔄 Process Flow

1. **Incoming Wafer Carrier**  
   Wafers arrive in a protective carrier that ensures they remain uncontaminated before entering the processing line.

2. **Wafer Inspection**  
   The wafers are visually and optically inspected for surface defects, contamination, or damage before further processing.

3. **Wafer Front Tape Lamination**  
   A protective tape is laminated on the front (device side) of the wafer to protect it during subsequent processes like grinding and dicing.

4. **Wafer Backside Grinding**  
   The wafer’s backside is ground using a rotating grinding wheel to reduce thickness and enable better thermal performance and flexibility for final packaging.

5. **Tape Frame Mounting to Wafer Backside**  
   After grinding, the wafer is mounted on a ring frame using an adhesive tape. This stabilizes the wafer and keeps individual die in place during dicing.

6. **Two-step Wafer Dicing (Laser Grooving + Blade Dicing)**  
   - **Laser Grooving**: Precision laser cuts grooves along scribe lines to weaken the wafer structure.  
   - **Blade Dicing**: A high-precision blade is then used to physically dice the wafer into individual dies or chips.

<img src="../images/module2/Screenshot 2025-04-05 165319.png" alt="Package Manufacturing Unit" width="600"/>
</details>

<details>
<summary> Wire Bond Packaging - Die Attach To Molding </summary>

# 🛠️ Activities Inside the Cleanroom Area – Wire Bond Packaging

This section covers the standard steps followed inside a cleanroom environment for **Wire Bond Packaging** in semiconductor device assembly.

---

## ⚙️ Process Flow

### 1. Die Attach
The individual chip (die) is attached to a substrate or lead frame using epoxy.  
Steps include:
- **Epoxy Dispense**  
- **Pick the Chip**  
- **Place on the Die Attach Film (DAF)**

---

### 2. Curing
The die-attached unit is subjected to a heating process to cure the epoxy, ensuring a strong and stable bond between the die and the substrate.

---

### 3. Wire Bonding
Fine gold or aluminum wires are bonded between the die and the package substrate pads using thermal and ultrasonic energy.

#### Key steps:
- Formation of a **ball bond** using an EFO (Electronic Flame-Off) spark  
- Bonding the ball to the die pad  
- Creating a **wire loop**  
- Forming a **crescent bond** on the substrate side

---

### 4. Molding (Transfer Molding)
A mold compound is injected to encapsulate the wire-bonded die, providing protection from environmental damage and mechanical stress. Resin flows uniformly to cover the entire chip.

---

### 5. Marking (Laser)
Laser marking is used to engrave identification codes, logos, or batch numbers on the molded package surface.

---

### 6. Singulation (Dicing Blade)
The molded wafer is cut into individual units (ICs) using a **dicing blade**. A thinner blade is typically used to minimize chipping and maximize precision.

---

<img src="../images/module2/Screenshot 2025-04-05 170414.png" alt="Package Manufacturing Unit" width="600"/>

</details>

<details>
<summary> Flip Chip Assembly - Bump Formation And Underfill </summary>

# Activities Inside the Cleanroom Area

## 📦 Flip Chip Packaging

Flip chip packaging is a semiconductor packaging method that involves mounting the die face-down on the substrate, which improves electrical performance and allows for more interconnects.

### 🔩 Key Steps:

1. **Bump Formation on Silicon (Si)**
   - Solder bumps are created on the die.
   - Bumps are reflowed to form strong electrical and mechanical connections.

2. **Chip Flip and Placement**
   - The chip is flipped upside down.
   - Solder balls align with the substrate’s bond pads.
   - Flux is applied to promote solder wetting.

3. **Solder Reflow**
   - The chip is heated so the solder balls melt and bond with the substrate.

4. **Flux Cleansing**
   - Residual flux is removed using solvent spray to prevent corrosion.

5. **Underfill Dispensing and Cure**
   - Underfill material is applied to improve mechanical strength and thermal conductivity.
   - Heating cures the underfill.

6. **Molding and Marking**
   - A protective mold compound is applied.
   - Laser marking is done for identification.
   
7. **Ball Mounting and Reflow**
   - Solder balls are mounted on the substrate.
   - A final reflow process ensures firm attachment of solder balls.

---
<img src="../images/module2/Screenshot 2025-04-05 170948.png" alt="Package Manufacturing Unit" width="600"/>

</details>

<details>
<summary> Wafer Level Packaging And Conclusion </summary>

## 🧩 Wafer Level Packaging (WLP)

Wafer Level Packaging is a technology that enables the packaging of ICs while still in the wafer format, leading to smaller size and lower cost.

### 🔁 Reconstitution Process:

1. **Diced Wafer Handling**
   - Known good dies are picked and placed onto a temporary carrier.

2. **Molding**
   - Dies are molded into a single reconstituted wafer.
   - The carrier is later released, leaving a molded wafer.

### 🔧 RDL (Redistribution Layer) Preparation:

1. **Dielectric & Metal Coating**
   - Initial dielectric and metal layers are deposited on the reconstituted wafer.

2. **RDL Patterning**
   - Multiple RDL layers are patterned for interconnection routing.

3. **Solder Ball Attach**
   - Solder balls are mounted on the final RDL pads to enable surface mounting.

4. **Final Laser Marking and Singulation**
   - Each packaged die is marked.
   - The wafer is diced (singulated) into individual packages.

---
<img src="../images/module2/Screenshot 2025-04-05 171040.png" alt="Package Manufacturing Unit" width="600"/>

