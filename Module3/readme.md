<summary> <h2> Labs: Thermal Simulation of Semiconductor Packages with ANSYS </h2> </summary>

# 🧊 Ansys Icepak Lab – Initial Setup & Creating a Flipchip BGA Package

This guide walks through the initial steps for setting up an Ansys Icepak thermal simulation and adding a Flipchip BGA package component.

---

# Thermal Analysis of a Flipchip BGA in Ansys Icepak

This README provides a step-by-step guide to perform a thermal analysis of a Flipchip BGA package using Ansys Icepak. The simulation is performed for a power input of 1 W.

---

## 🛠️ Step 1: Insert Icepak Design

- Open **Ansys Workbench**.
- Navigate to `Project` -> `Insert Icepak Design`.

---

## 🧭 Step 2: Open the Icepak Layout

- Click the **Icepak** tab in the top toolbar to launch the Icepak layout environment.

---

## 📦 Step 3: Create a Flipchip BGA Package

- Go to `Icepak` -> `Toolkit` -> `Geometry` -> `Packages` -> `Flipchip_BGA`.
- A configuration window will appear.
- Set parameters:
  - **xLength**: 15 mm
  - **yLength**: 15 mm
  - **Package Thickness**: 3 mm
  - **Model Type**: Detailed
  - **Symmetry**: Full
- Click **OK** to generate the 3D model.
- The model will now appear in the working space.

---

## 📂 Step 4: Explore the Model Structure

- In the **Model Tree**, expand the **Solids** section to view:
  - `Substrate`
  - `Die`
  - `Underfill`, etc.

---

## ♨️ Step 5: Assign Thermal Power

- Navigate to `Project Manager` -> `Thermal`.
- Enter the **Power** value (e.g., `1 W`) and click **OK**.

---

## 🌡️ Step 6: Assign Thermal Sources

- In `Solids`, select `Flipchip-BGA1_substrate`.
  - Right-click -> `Assign Thermal` -> `Source`.
  - In the dialog box, set **Thermal Condition** to `Ambient Temperature`.
  - Click **OK**.
- Delete any extra element like `Flipchip_BGA_trace1` under the Thermal node.

---

## 📈 Step 7: Assign Temperature Monitors

- In `Solids`, select `Substrate` -> `Assign Monitor` -> `Point`.
  - Tick **Temperature** -> Click **OK**.
- Repeat the same process for the **Die** and **Underfill** components.

---

## 🧩 Step 8: Generate Mesh

- Go to the **Mesh** tab.
- Click `Simulation` -> `Generate Mesh`.
- Save the file when prompted -> Click **OK**.

---

## 🔍 Step 9: Inspect Mesh Quality

- In **Mesh Visualization**, click `Quality`.
- Check parameters such as:
  - **Face Alignment**
  - **Skewness**
  - **Volume**

---

## ✅ Step 10: Validate the Setup

- Click `Validate` from the top menu bar.
- Ensure all validation checks return **green ticks**.
- This confirms the setup is ready for simulation.

---

## 📊 Step 11: Run Simulation and Plot Temperature Field

- Click `Analyze All` from the top bar.
- Select the **Flipchip BGA** package.
- Navigate to `Plot Field` -> Select `Temperature` -> Choose `Temperature`.

### Configure Output Options:

- Enable:
  - `Specify Name`
  - `Specify Folder`
  - `Plot on Surface Only`
- In `Surface Smoothing`, enable **Gaussian Smoothing**.
- Click **OK** -> then **Done**.

---

## ✅ Final Output

A thermal analysis of the **Flipchip BGA** package is successfully completed for a power input of **1 W**.

---

## 📸 Simulation Steps (Screenshots)

<table>
  <tr>
    <td><img src="../images/module3/Screenshot 2025-04-04 220321 - Copy.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 220321.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 220840 - Copy.png" width="250"/></td>
  </tr>
  <tr>
    <td><img src="../images/module3/Screenshot 2025-04-04 220840.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 221220 - Copy.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 221220.png" width="250"/></td>
  </tr>
  <tr>
    <td><img src="../images/module3/Screenshot 2025-04-04 221657 - Copy.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 221657.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 221825 - Copy.png" width="250"/></td>
  </tr>
  <tr>
    <td><img src="../images/module3/Screenshot 2025-04-04 221825.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 222041 - Copy.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 222041.png" width="250"/></td>
  </tr>
  <tr>
    <td><img src="../images/module3/Screenshot 2025-04-04 222103 - Copy.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 222103.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 222453 - Copy.png" width="250"/></td>
  </tr>
  <tr>
    <td><img src="../images/module3/Screenshot 2025-04-04 222453.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 222516.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 222746.png" width="250"/></td>
  </tr>
  <tr>
    <td><img src="../images/module3/Screenshot 2025-04-04 222453.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 223108.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 223300.png" width="250"/></td>
  </tr>
  <tr>
    <td><img src="../images/module3/Screenshot 2025-04-04 223415 - Copy.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 223415.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 223843.png" width="250"/></td>
  </tr>
  <tr>
    <td><img src="../images/module3/Screenshot 2025-04-04 223904.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 224148.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 224249.png" width="250"/></td>
  </tr>
  <tr>
    <td><img src="../images/module3/Screenshot 2025-04-04 224409.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 224954.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 225019.png" width="250"/></td>
  </tr>
  <tr>
    <td><img src="../images/module3/Screenshot 2025-04-04 225048.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 225112.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 225310.png" width="250"/></td>
  </tr>
  <tr>
    <td><img src="../images/module3/Screenshot 2025-04-04 225336.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 225509.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 225808.png" width="250"/></td>
  </tr>
  <tr>
    <td><img src="../images/module3/Screenshot 2025-04-04 225839.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 230328.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 235038.png" width="250"/></td>
  </tr>
  <tr>
    <td><img src="../images/module3/Screenshot 2025-04-04 235105.png" width="250"/></td>
    <td><img src="../images/module3/Screenshot 2025-04-04 235203.png" width="250"/></td>
    
  </tr>

</table>
