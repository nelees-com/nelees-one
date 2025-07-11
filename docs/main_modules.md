# Nelees Modular Module Types (v.1 status: proposal/draft)

This document outlines the simplified and premium-oriented modular architecture for the Nelees One ceiling system. All components are designed to work together seamlessly, giving users high configurability without compromising on aesthetics or performance.

## System Overview
Each hexagonal module is composed of four key layers:

1. **Backbone Chassis**
   - Physical skeleton for mounting
   - Includes AC passthrough and mechanical attachment
   - Hosts 220V to 24V power converter

2. **Main PCB**
   - Manages internal power distribution and connectivity (ESP32-S3 or simillar )
   - easy to replace (future upgrades)

3. **Functional PCB**
   - Depends on module type: LEDs pannel, WiFi, audio,  etc.
   - easy to install / replace

4. **Custom Edges**
   - Vented, solid, translucent, or textile
   - May contain RGB LEDs, sensors, or be dummy for aesthetics
   - vertical edges for peripheric hexagones (interior hexagons don't use them: cable management, airflow). 


---

## Module Types

### 🟡 Illumination Module
**Purpose:** Main lighting for the space

- **LED Panel Options:**
  - Warm/Cold White (High Lumen, Power LEDs)
  - RGBW Mood Lighting (Sex Scene Ready™)
- **Mounting Surface:** Translucent diffuser (or side-edge orientation , unlikely because of thermal concerns ...but who knows?  )
- **Edge Sensors:** Only if thermal isolation is ensured

### 🟠 RGB/Ambient Module
**Purpose:** Mood lighting, atmospheric control, sensor integration

- **LEDs:** RGBW strips, low thermal output
- **Housing:** Translucent or textile finish
- **Edge Sensors:** recommended

- 
### 🔵 Network/Audio Module
**Purpose:** Smart connectivity or sound system

- **Variants:**
  - WiFi AP / Zigbee / LoRa / BLE Gateway
  - Smart Speaker
- **Positioning:**
  - Rear-mounted PCB (low thermal)
  - Behind **textile front face** for audio and signal transparency
- **LED Layer:** Optional RGBW grid behind textile

---

- 
## Edges Types

### 1.Dummy 
**Purpose:** design / air vent

### 2.Sensor Hub
**Purpose:**  Ambient sens
  - Temperature
  - Humidity
  - VOC
  - CO₂
- **Sensor Positioning:**
  - Mounted in **edge caps**, thermally insulated from the core
  - **Exposed to ambient air** via vented or open-side modules

### 3. RGB LED 
**Purpose:**  design



---

## Design Notes
- All modules share same physical interface and power input.
- Module architecture allows clean stacking and function separation.
- Edge modules support passive cooling and sensor exposure.
- Thermal Throttling Logic can adjust LED power in centrally located modules.
- Panes can be changed by user: translucent for light, textile for audio and ambient.
