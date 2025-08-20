# 📸 LogiCam - Digital Circuit Analyzer and Verilog Code Generator
An edge-deployable system that scans hand-drawn or printed logic  circuits via phone's camera, detects logic gates using deep learning,
assigns variables to input and output connections, and generates the corresponding Boolean expression.
Additionally, the system also generates the equivalent Verilog code for simulation.

---

## Features
- Captures digital logic circuit diagrams using a phone camera
- Detects logic gates using a YOLOv8n-TFLite model
- Parses corresponding Boolean expression for the circuit
- Generates Verilog code for simulation
- Real-time processing on Android platform

---

## System Architecture

The system consists of the following main components:

1. **Image Capture**  
   Uses the phone camera to capture hand-drawn or printed digital logic circuits.

2. **Logic Gate Detection**  
   A YOLOv8n-TFLite model runs on-device to detect logic gates such as AND, OR, NOT, NAND, NOR, XOR, and XNOR.

3. **Connection Parsing and Variable Assignment**  
   Analyzes spatial relationships between gates to identify input/output connections and assigns variables accordingly.

4. **Boolean Expression Generation**  
   Constructs the Boolean expression by traversing the logic graph derived from gate connections.

5. **Verilog Code Generation**  
   Converts the parsed Boolean logic into Verilog HDL code for simulation and verification.

---

## System Framework

![Screenshot 2025-06-05 115407](https://github.com/user-attachments/assets/b692d313-93c3-43a9-b609-2270e11c5eb9)

## Validation
### A. Test Circuit
![Picsart_25-06-05_12-10-51-146](https://github.com/user-attachments/assets/6bbd7721-aded-491e-857b-2d5dc7b60b2a)

### B. Logic Gate Detection on Android App
![WhatsApp Image 2025-06-04 at 12 33 38_34833f83](https://github.com/user-attachments/assets/47e918db-1892-4c0b-8bda-2a062834c8b4)

### C. Variable Assignment and Logic Parsing
![Picsart_25-06-05_12-10-27-953](https://github.com/user-attachments/assets/9f12edb6-3276-4b94-86c9-dc5284a64545)

### D. Boolean Expression Output
✅ **(_NOT_ (C _AND_ D)) _OR_ (A _OR_ B)**

### E. Verilog HDL Code Generation
![Picsart_25-06-05_12-11-28-125](https://github.com/user-attachments/assets/2bf60a80-4899-4162-92bf-d2553df2ee3b)

![Picsart_25-06-05_12-14-42-110](https://github.com/user-attachments/assets/00aef1a6-17a1-4829-8fac-b0aa2500d6f6)

## Contributing Teammates
- [E Sujaya](https://github.com/Sujaya-E)
- [Shashank Padavalkar](https://github.com/Shashank-Padavalkar)
- Sambhram Doddamane
