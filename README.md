# **Propeller Calculator for Wageningen B-Series Propellers**

## **Code Overview**
This Python-based implementation analyzes marine propellers using the Wageningen B-series data. It provides tools to calculate performance metrics such as **thrust coefficient (K_T)**, **torque coefficient (K_Q)**, and **advance ratio (J)**, essential for evaluating propeller efficiency in marine applications. Run on Jupyter Notebook.

---

## **Core Features**

### **1. Propeller Calculator Class**
The `PropellerCalculator` class encapsulates all functionality for propeller performance analysis. Key methods include:
- **`calculate_advance_ratio()`**: Calculates the advance ratio (\(J\)) based on speed, wake fraction, diameter, and revolutions.
- **`calculate_KT()`**: Computes the thrust coefficient (\(K_T\)) using polynomial expressions with pre-defined coefficients.
- **`calculate_KQ()`**: Computes the torque coefficient (\(K_Q\)) using similar methods for torque.
- **`calculate()`**: A wrapper function integrating all calculations to compute \(K_T\), \(K_Q\), and \(J\) for given inputs.

### **2. Polynomial Expressions**
The code utilizes polynomial equations derived from Wageningen B-series data to compute thrust and torque coefficients using pre-defined coefficients stored in the class.

### **3. Input Parameters**
The calculator takes essential parameters to derive the curves:
- **Propeller Specifications**: Diameter (D), pitch (P), number of blades (Z), blade area ratio (\(A_e/A_o\)), thickness-to-chord ratio (t/c).
- **Operating Conditions**: Speed (\(V\)), wake fraction (\(w_T\)), and fluid density (\(\rho\)).

### **4. Visualization**
The notebook integrates `matplotlib` for visualizing efficiency curves and other performance metrics, for result interpretation.

---

## **Example Workflow**
1. **Define Input Parameters**:
    - Specify speed, wake fraction, diameter, number of blades, etc.
2. **Run the Calculator**:
    - Use the `calculate()` method to compute \(K_T\), \(K_Q\), and \(J\).
3. **Analyze Results**:
    - Print or plot the results to evaluate performance.
4. **Further Analysis**:
    - key additional parameters into the reference calculator to observe deeper performance metrics.
5. **Optimize Design**:
    - Adjust parameters and re-run calculations for better performance metrics.
---


**Done by**: marcustzy
