# College-final-year-project
AC to DC voltage &amp; current controller, electronic circuit

### Project Explanation:  

<p align="center">
  <img src="https://github.com/user-attachments/assets/ce51721e-c143-4cb3-997e-a8593c4d5aae" alt="Image 1" width="46%" style="margin-right: 10px;"/>
  <img src="https://github.com/user-attachments/assets/edee84d4-9eef-4ef1-b90c-00a30bd90d70" alt="Image 2" width="46%" style="margin-left: 10px;"/>
  </br>
  <img src="https://github.com/user-attachments/assets/aa7aaf62-3a21-4960-b7e4-1d61de96f6e7" alt="Image 1" width="59%" style="margin-right: 10px;"/>
  <img src="https://github.com/user-attachments/assets/d817fe35-f973-400e-8ee7-28f1d8b26b1a" alt="Image 2" width="33%" style="margin-left: 10px;"/>
  </br>
  <img src="https://github.com/user-attachments/assets/5fd97c4f-7415-46dc-8982-9924256a78c7" alt="Image 1" width="52.5%" style="margin-right: 10px;"/>
  <img src="https://github.com/user-attachments/assets/4b4111c5-0dcb-404a-9017-11a3c0eb603f" alt="Image 2" width="39.5%" style="margin-left: 10px;"/>
  </br>
</p>

https://github.com/user-attachments/assets/46bedf4e-fc17-4426-94a9-905563ad5ae5

**Input Power:**
1. The circuit starts with an AC mains input of **230V at 50Hz (Indian frequency)**.
2. The input is connected to a **transformer** (rated for 230V to the desired secondary voltage and 1.5A capacity).  
   - This step-down transformer reduces the voltage to a manageable level (as per your circuit design).  

---

https://github.com/user-attachments/assets/000175be-9e58-4870-9e30-905f1b571046

**Rectification Stage:**
3. The reduced AC voltage from the transformer is fed into a **full-wave rectifier circuit**, which is built using four **6A4 diodes** in a bridge configuration.  
   - The rectifier converts AC to pulsating DC.  

---

**Smoothing Stage:**
4. A **470μF capacitor (35V)** is connected after the rectifier to smoothen the pulsating DC into a stable DC output.  
   - This capacitor filters out most of the ripples.  

---

**Voltage Regulation Stage:**
5. The rectified and filtered DC is fed into **voltage regulator ICs (7815 and 7805)** for precise voltage outputs of **+15V** and **+5V**, respectively.  
   - These ICs ensure stable voltage outputs for different components in the circuit.  

---

**Cooling Mechanism:**
6. To prevent overheating of the components, a **heat sink** is attached to the voltage regulators. Additionally, a **cooling fan** is integrated to dissipate heat efficiently.  

---

**Output Stage:**
7. The circuit includes a **300W 10A 30V Buck Converter**, which adjusts the output voltage and current to meet the load's requirements.  
   - This component handles high power efficiently but is limited by the **5-8A current range**, as exceeding this will cause the circuit to overheat or fail.  

---

**Control and Switching System:**
8. **Potentiometers (10kΩ)** are included for fine-tuning voltage and current levels.
9. **LED indicators** are used for status indication.  
10. **Display module** shows the output voltage and current for monitoring purposes.  

 
### ✅ **Control and Switching System**
1. **Potentiometers (10kΩ)**:  
   - **Purpose**: To regulate voltage and current for the electroplating process.  
   - **Connections**:  
     - One potentiometer controls the **voltage** output from the buck converter.  
     - The other potentiometer controls the **current** flowing to the output probes (alligator clips connected to the cathode and anode).  

2. **Black Switch**:  
   - **Purpose**: Master switch to turn the entire power supply system ON or OFF.  
   - **Connection**: Connected to the **primary side of the transformer**. Switching it ON energizes the entire system.  

3. **Red Switch**:  
   - **Purpose**: Controls the output probes (cathode and anode). It allows you to start or stop the electroplating process without turning off the whole system.  
   - **Connection**: Placed on the output side after the buck converter, controlling power to the **alligator clips**.  

---

### **Display System**
4. **Digital Display (Voltmeter + Ammeter)**:  
   - **Purpose**: Tracks the real-time voltage and current supplied to the electrolyte solution during the electroplating process.  
   - **Connections**:  
     - Voltage input is taken from the **buck converter output**.  
     - Current is measured using a **shunt resistor** in series with the output probes.  

---

### **LED Indicators**
5. **Red LED (Process Indicator)**:  
   - **Purpose**: Indicates that the electroplating process has started, i.e., current is flowing through the electrolyte.  
   - **Connection**:  
     - Connected in **series** with the electrolyte and the alligator clips.  
     - It lights up only when the circuit is complete, and current flows through the electrolyte solution.  

6. **Other LEDs (Status Indicators)**:  
   - There are **two additional LEDs** for general status indication (e.g., power ON/OFF).  
   - Connections:  
     - One LED is connected to the output of the **black switch** to indicate the system is ON.  
     - The second LED may indicate the buck converter is powered.  

---

### Electroplating Process Details  
- **Electrolyte Solution**:  
  - Nickel Sulfate (**NiSO₄**) - 10 g/L.  
  - Oxalic Acid - 10 g/L.  
  - 200 mL of distilled water.  

- **Measured Parameters**:  
  - **Voltage**:  
    - 11.8V when the circuit is incomplete (open).  
    - 5.9V during the electroplating process (closed circuit).  
  - **Current**: 0.13A during the process.  

- **Weight Changes**:  
  - **Initial Weight**: 3.418g (before cleaning with acid).  
  - **Final Weight**: 3.314g (after the electroplating process).  

---

### Circuit Precautions:
- The system is designed to handle up to **5-8A current**; exceeding this limit can burn out the components (e.g., wires, capacitors).  
- Ensure proper insulation and cooling to avoid electrical hazards.  
- Use high-quality **soldering wire and connections** to maintain circuit integrity.  

---

### Total Cost Breakdown:  
As per your shared list, the total cost of the project is **₹3245**, including components and repair expenses. [Learn more](https://college-final-year-project.netlify.app/)

![IMG_5137](https://github.com/user-attachments/assets/f3f10e1e-accc-4160-8502-3710beded13a)


<div style='display:flex; align-items:center; gap: 30px;' align='center'>

# Update with Resistors (limit 9V 4amp) - March 2025
</div>

<p align="center">
  <img src="https://github.com/user-attachments/assets/315dab46-ac37-4b29-8788-19aad9768e5d" alt="Image 1" width="45%" style="margin-right: 10px;"/>
  <img src="https://github.com/user-attachments/assets/e91bcefa-8744-40a2-a793-f8c5cf71e4ad" alt="Image 2" width="45%" style="margin-left: 10px;"/>
  </br>
  <img src="https://github.com/user-attachments/assets/095e444a-4207-4657-865e-f9c2176fe043" alt="Image 1" width="45%" style="margin-right: 10px;"/>
  <img src="https://github.com/user-attachments/assets/251fd80d-a1f1-4f0c-ab09-1ca3f4650ef0" alt="Image 2" width="45%" style="margin-left: 10px;"/>
  </br>
  <img src="https://github.com/user-attachments/assets/2348bcf1-4032-46fb-b775-de3435e60bc2" alt="Image 1" width="45%" style="margin-right: 10px;"/>
  <img src="https://github.com/user-attachments/assets/19b84d16-55da-4cc6-98f3-56b391a1d635" alt="Image 2" width="45%" style="margin-left: 10px;"/>
  </br>
  <img src="https://github.com/user-attachments/assets/4ca34ca0-601d-4b53-bf86-76944c04b123" alt="Image 1" width="45%" style="margin-right: 10px;"/>
  <img src="https://github.com/user-attachments/assets/17fcc9fa-0eaf-40d7-8155-30d04730a748" alt="Image 2" width="45%" style="margin-left: 10px;"/>
  </br>
</p>

## after using 9V 4 amp, this is happns

![resistors](https://github.com/user-attachments/assets/daa643e7-bf54-4855-9d06-89380113a25d)

---

# Alternate Circuit

https://github.com/user-attachments/assets/6a481bc7-f602-4173-9d15-df8144aa25de

---

</br>
</br>

<div style="display: flex; align-items: center; gap: 10px;" align="center">
  
## ⭐ Data & Result ⭐
</div>

# This is not the full repo --> This is a small part of our project, actual data is in a Private repo 🔐 [link](https://github.com/akashdip2001/college-final-year-project-lock/blob/main/README.md)

![002](https://github.com/user-attachments/assets/da4c8753-77ce-4fd8-8e4a-b444804193d6)
