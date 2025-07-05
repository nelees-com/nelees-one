# Nelees One – Modular AC Power Architecture

## 🔌 Concept Summary

Each hexagon module includes an integrated and certified AC-DC power supply (220V → 24V). The system is designed to pass 220V AC between modules in a daisy-chain fashion using dedicated IN/OUT connectors. No central power supply is required.

---

## 🎯 Design Objectives

- Fully modular and scalable design
- Simplified installation and extension
- No centralized power hub
- Certified safety and EMI-compliant power blocks
- Plug-and-play architecture

---

## 🔲 Hexagon Power Module

**Each module includes:**
- **AC IN:** 220V input from previous module or wall
- **AC OUT:** 220V passthrough to next module
- **Integrated AC-DC converter:** 220V AC to 24V DC (e.g. HDR-30-24)
- **Internal 24V DC bus:** for LED and control electronics

---

## 🔁 AC Daisy-Chain Topology

- Standardized 2-pin or 3-pin connectors (L/N or L/N/PE)
- Up to 20 modules per 10A circuit
- All AC-DC converters are fully certified and enclosed
- Minimal voltage drop due to low current per module (~0.1A at 220V)

---

## ⚠️ Safety Features

- Internally fused and protected AC-DC converters
- Optional additional PTC or inline fuse per module
- Proper strain relief and locking connectors
- Enclosure designed to comply with safety regulations (CE/UL)

---

## 🧩 Mechanical and Electrical Interface

| Connector | Pins | Function             |
|-----------|------|----------------------|
| AC IN     | 2/3  | 220V Line + Neutral (+ PE optional) |
| AC OUT    | 2/3  | 220V passthrough     |
| DC Rail   | —    | Internal 24V distribution only |

---

## 🛠 Integration Notes

- Modules can be added or removed without altering the power topology
- 220V routed safely in enclosure with proper isolation
- No logic or communication required in power subsystem

---

## 🔧 Schematic Layout Concept

```
[AC_IN]──(to certified 220V AC → 24V DC block)──[AC_OUT]
             │
         [24V DC BUS]
             │
        [LED / Logic Loads]
```

---

## ✅ Benefits

- Certified safety with minimal design complexity
- Maximum flexibility for dynamic lighting layouts
- No centralized failure point
- Compatible with mass production and retrofit installation

---
