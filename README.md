# PACEPOD

**PacePod – Summary and Key Features**

**What is the PacePod?**
The PacePod is a small, wearable, low-power embedded device designed to help athletes maintain a target **cadence** (e.g., running steps per minute or rowing strokes per minute). It measures the athlete’s movement events in real time and provides simple **audio feedback** to guide them toward their desired pace.

---

### **Key Features**

**1. Wearable & Flexible Placement**

* Compact and lightweight.
* Can be worn on the **wrist, neck, or ankle**, depending on the activity.
* Designed to work across multiple sports and exercises.

**2. Simple Input System**

* Receives a clean electrical pulse from an external sensor (e.g., accelerometer or switch).
* Each pulse represents one movement event (step, stroke, etc.).
* Uses **interrupt-driven input** for accuracy and low power use.

**3. Cadence Measurement**

* Calculates cadence by measuring time between events.
* Operates in real time with high reliability.
* Compares actual cadence to a user-set target.

**4. Audio Feedback**

* No sound if cadence is within tolerance (e.g., ±2% of target).
* **Low-pitch beep** if cadence is too slow.
* **High-pitch beep** if cadence is too fast.
* Distinct warning pattern for low battery.

**5. Minimal User Interface**

* A **single button** to cycle through states:

  * Off
  * Standby / Pace-Set
  * Active / Pacing

**6. Low-Power Operation**

* Designed for long battery life.
* Uses sleep modes and interrupt-based operation.
* Enters deep sleep or safe shutdown when battery is critically low.

**7. Data Logging**

* Periodically stores cadence with elapsed time.
* Uses limited internal memory (RAM/EEPROM/Flash).
* Must handle memory-full conditions (e.g., stop logging or overwrite old data).

**8. Data Retrieval**

* Logged data can be transferred to a PC or external device.
* Uses a **1-Wire communication protocol** over a single GPIO pin.

**9. Reliability & Fault Handling**

* Graceful handling of:

  * **Memory full** conditions.
  * **Low battery** detection with warning and safe shutdown.
* Designed to avoid abrupt failure or battery damage.

