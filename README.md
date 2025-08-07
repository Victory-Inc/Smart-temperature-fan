
# 🌬️ Temperature-Activated SmartFan

## 📘 Description

This project is a **Temperature-Activated SmartFan** designed to respond to heat by turning on an LED. When the LED is on, it signals that the temperature has passed a certain threshold and allows the user to press a button to activate the fan motor. It can be built using either discrete components or a HW-130 Motor Shield.

---

## 🧰 Parts Used

### Option 1: Using Discrete Components

- 1x Red LED  
- 1x Fan Motor  
- 1x Push Button  
- 1x TIP120 Transistor  
- 1x 9V Battery  
- 1x Temperature Sensor (e.g., TMP35/TMP36)  
- 1x Diode (e.g., 1N4001 or 1N4148)  
- 2x 20Ω Resistors  
- 17x Jumper Wires  

### Option 2: Using HW-130 Motor Shield

- 1x LED  
- 1x HW-130 Motor Shield  
- 1x Push Button  
- 1x 1kΩ Resistor  
- 1x 10kΩ Resistor  
- 1x Temperature Sensor  
- 1x Fan Motor  

---

## ⚙️ How It Works

1. **Temperature Detection:**  
   The temperature sensor measures the ambient temperature and sends an analog voltage to the Arduino (or controller). When the temperature rises past a defined threshold, the system "arms" itself.

2. **Visual Cue (LED):**  
   Once the threshold is reached, the LED turns on to indicate the system is ready. This gives the user feedback that the temperature is high enough to allow fan activation.

3. **Button Activation:**  
   With the LED lit, pressing the button sends a signal to activate the fan motor. This allows manual control even in an automated system, providing flexibility and safety.

4. **Motor Control:**  
   Depending on the version:
   - **Discrete version:** The TIP120 transistor acts as a switch, allowing the fan to draw power from the 9V battery when activated.
   - **Motor Shield version:** The fan is powered through one of the shield's motor outputs, controlled by digital signals.

---

