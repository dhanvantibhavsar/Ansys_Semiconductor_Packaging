
<summary> <h2> Package Design and Modeling: Building a Semiconductor Package from Scratch </h2> </summary>

# 🧊 Create the Semiconductor package cross-section in Ansys AEDT

This lab focuses on designing a semiconductor wire bond package from scratch using **Ansys Electronics Desktop (AEDT)**. The objective is to model the complete cross-section of a wire bond package, including die, substrate, bonding wires, and mold compound.

---

## Steps to Model the Wire Bond Package

### 1. Start a New Project
- Launch **Ansys Electronics Desktop**.
- Select **Q3D Layout Design** to start.

### 2. Create the Die
- Use the **Modeler → Surface → Rectangle** option.
- Define the **die thickness**: `0.2 mm`.
- Rename the rectangle as `die`.
- Assign **Material**: `Silicon`.

### 3. Create the Substrate
- Again, draw a rectangle.
- Set the **size**: `5 mm x 5 mm`.
- **Thicken the rectangle** to represent the substrate: `-0.5 mm`.
- Rename this object as `substrate`.
- Move the **die** on top of the substrate by adjusting its position to `(x = -1, y = -1, z = -0.1)`.

### 4. Add Die Attach Layer
- Create another rectangle **same size as die** at origin `(0, 0, 0)`.
- Set **thickness**: `-0.1 mm`.
- Assign appropriate **material** **modified_epoxy** for thermal conductivity simulation. 

### 5. Add Die Pad
- Create a thin rectangle to represent the **die pad**.
- Set **thickness**: `0.005 mm`.

### 6. Add Bond Pads
- Create bond pads on both die and substrate.
- These will serve as connection points for the wire bond.
- Assign **material** (typically metal, e.g., gold or aluminum).

### 7. Connect with Bond Wires
- Use the **Bondwire tool**.
- Connect the **die pads to substrate pads** using **gold wire**

### 8. Add Mold Compound
- Add a rectangular mold compound to encapsulate the die and wire bonds.
- Set **thickness**: `1.2 mm`.
- Assign mold material (e.g., epoxy molding compound).

---

## 📸 Simulation Steps (Screenshots)

<table>
  <tr>
    <td><img src="../images/module5/Screenshot 2025-04-06 131303.png" width="250"/></td>
    <td><img src="../images/module5/Screenshot 2025-04-06 131442.png" width="250"/></td>
    <td><img src="../images/module5/Screenshot 2025-04-06 132339.png" width="250"/></td>
    <td><img src="../images/module5/Screenshot 2025-04-06 132505.png" width="250"/></td>
  </tr>
  <tr>
    <td><img src="../images/module5/Screenshot 2025-04-06 132817.png" width="250"/></td>
    <td><img src="../images/module5/Screenshot 2025-04-06 133220.png" width="250"/></td>
    <td><img src="../images/module5/Screenshot 2025-04-06 133459.png" width="250"/></td>
    <td><img src="../images/module5/Screenshot 2025-04-06 133928.png" width="250"/></td>
  </tr>
  <tr>
    <td><img src="../images/module5/Screenshot 2025-04-06 134222.png" width="250"/></td>
    <td><img src="../images/module5/Screenshot 2025-04-06 134416.png" width="250"/></td>
    <td><img src="../images/module5/Screenshot 2025-04-06 134600.png" width="250"/></td>
    <td><img src="../images/module5/Screenshot 2025-04-06 135030.png" width="250"/></td>
  </tr>
  <tr>
    <td><img src="../images/module5/Screenshot 2025-04-06 135609.png" width="250"/></td>
    <td><img src="../images/module5/Screenshot 2025-04-06 135910.png" width="250"/></td>
    <td><img src="../images/module5/Screenshot 2025-04-06 140009.png" width="250"/></td>
    <td><img src="../images/module5/Screenshot 2025-04-06 140551.png" width="250"/></td>
  </tr>
  <tr>
    <td><img src="../images/module5/Screenshot 2025-04-06 140720.png" width="250" height="220"/></td>
    <td><img src="../images/module5/Screenshot 2025-04-06 141327.png" width="250"/></td>
    <td><img src="../images/module5/Screenshot 2025-04-06 141843.png" width="250"/></td>
    <td><img src="../images/module5/Screenshot 2025-04-06 141936.png" width="250"/></td>
  </tr>
  <tr>
    <td><img src="../images/module5/Screenshot 2025-04-06 142156.png" width="250"/></td>
  </tr>
  </table>

