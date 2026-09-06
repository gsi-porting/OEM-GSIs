# 🌐 OEM GSI Collection

A modern, Material You-themed web index hosting a curated collection of Generic System Images (GSIs) ported from various OEM ROMs (Samsung OneUI, Xiaomi HyperOS/MIUI, OnePlus OxygenOS, Google Pixel, ColorOS, RealmeUI, and RisingOS).

---

## ⚠️ Important Note
> **The website/index lists ROMs by their source device names (e.g., *S9*, *Mi 8*, *OnePlus 11*).** 
> 
> **These are NOT device-specific flashable zips for those models.** They are **GSIs** ported from those respective devices. Simply browse the collection, download the OS version you want, and **extract the archive** to get the core GSI image file (`.img`) for Project Treble flashing.

---

## 🎨 Features
* **Material You (MD3) Design:** Clean, responsive interface featuring dynamic color-picker themes and automatic dark/light mode switching.
* **OEM Tab Navigation:** Easily switch between OneUI, HyperOS/MIUI, Pixel, OxygenOS, RisingOS, ColorOS, and RealmeUI.
* **Version Sorted:** GSIs are neatly organized by Android versions and major software iterations.
* **Architecture Tags:** Explicitly marked tags for special architectures (such as `arm-v7a` and `arm-v9`) where applicable.

---

## 🛠️ General Flashing Guide
*Disclaimer: Flashing GSIs carries risks. Make sure your bootloader is unlocked, your device supports Project Treble, and you take a full backup before proceeding.*

1. **Unlock Bootloader:** Ensure your device's bootloader is unlocked.
2. **Download & Extract:** Download the GSI archive for your desired OEM/version from the collection and extract it to get the `system.img` (or similar `.img` file).

   **Make Sure:** Your Kernel Is Permissive Or It can Cause Bootloop And to make it permissive Use permissier-v5.zip
4. **Boot into Fastboot / Fastbootd:** Connect your phone to a PC and boot into fastboot mode.
5. **Flash the GSI:**
   ```bash
   fastboot flash system system.img
