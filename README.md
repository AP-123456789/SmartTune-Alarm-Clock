# SmartTune Alarm Clock - CAD Enclosure Project

Repository containing the 3D CAD model for the SmartTune Alarm Clock enclosure, designed entirely from scratch in Onshape as a learning project focused on parametric modeling, multi-part assemblies, and product design principles. The primary goal was to build a compact, modern desktop device enclosure that looks like a real manufactured product while ensuring sufficient internal clearance for future electronics.

---

## Key Features

* **Modern Enclosure Body**: A sleek 150 mm x 60 mm rectangular body with smooth filleted outer corners.
* **Recessed Display & LED Frame**: A dedicated front display recess paired with a thin custom-carved groove designed to house an RGB LED strip.
* **Embossed Time Display**: Manual text stamping of the static digits `07:40` with a clean 3D depth to simulate an active screen.
* **Control Buttons & Rear Venting**: Four front-facing button wells and a rear acoustic speaker grille featuring a clean 4x5 grid of 20 vent holes.
* **Packed Side Panel**: Fully loaded side profile featuring a standard USB port, an AUX audio jack, a charging indicator (`CHG`), a physical power switch (`ON | OFF`), and custom text labels.
* **Removable Back Cover & Fasteners**: A separate removable rear cover (Part 2) designed with a -1mm offset fit, supported by internal mounting posts and realistic assembly screws.

---

## Project Visuals & Work in Progress

### Initial Body & Extrusion
![Image 2](https://halflife.hackclub-assets.com/hackclub-half-life/sessions/OcYWjcDouGEzidswYkZNmkY7iSde7Zal/f7c4b6b026a0f461fafaf9c3ff9781fb94843ba06c8e0c3d0d1a4eab3dd82935.jpg)

### Display Recess & Button Wells
![Image4](https://halflife.hackclub-assets.com/hackclub-half-life/sessions/OcYWjcDouGEzidswYkZNmkY7iSde7Zal/ab6db1a84eac41b9a8dce74a667e5a207515eb72fd730fad1393c54b15fe1851.jpg)

### Rear Speaker Grille
![Image6](https://halflife.hackclub-assets.com/hackclub-half-life/sessions/OcYWjcDouGEzidswYkZNmkY7iSde7Zal/9d365a9556895ceafc0a7ccca4313d1361558a76b74f7eec253d0e0fd0e59c51.jpg)

### Side Panel Features & Labels
![Image22](https://halflife.hackclub-assets.com/hackclub-half-life/sessions/OcYWjcDouGEzidswYkZNmkY7iSde7Zal/416b4b6bfb3536cc6e2c50dd1ed7acc659850e0a1649baa8c746bd36bfa0034b.jpg)

---

## Design Process & What I Learned

Building this project involved a major learning curve and trial-and-error troubleshooting:

### Workspace Orientation & Reference Planes
Getting used to Onshape's view cubes and figuring out how to hide default planes (Front, Top, Right) when they cluttered the workspace. Reference guide used: Onshape Learning Center (https://cad.onshape.com/help/Content/sketch.htm).

### Dimension vs. Measure Tools
Overcoming initial confusion over dimension readings by learning that the **Dimension tool** sets sketch sizes, while the **Measure tool** only checks distances between selected edges or faces.

### Troubleshooting Intersection Errors
Encountering the frustrating red warning—`"Selected tools and targets do not intersect"`—when trying to cut button and display recesses. Learned how to fix this by ensuring sketches are attached directly to solid faces and managing merge scopes properly. Forum reference used: Onshape Community Forums (https://forum.onshape.com/).

### Thin-Wall Sketch Boundaries
Managing inner and outer sketch loops to carve the thin rectangular groove for the RGB LED strip instead of accidentally filling it in as a solid block.

### Multi-Part Assemblies & Hardware Fasteners
Transitioning from Part Studios to an Assembly tab (`Assembly 1`), inserting standard hardware components from Onshape libraries, and applying **Fastened mates** to secure the back cover without geometry collisions. Reference guide used: Onshape Standard Content Library (https://cad.onshape.com/help/Content/Standard-content/standard-content.htm).

---

## BOM

| Item | Purpose | Qty | Unit Price | Total Price | Vendor | Sourcing Link |
| :--- | :--- | :---: | :---: | :---: | :---: | :--- |
| **Screws (M3 x 8mm, 10-pack)** | Secure the removable rear cover to internal mounting posts | 1 | $1.95 | $1.95 | Adafruit | [Adafruit #4209](https://www.adafruit.com/product/4209) |
| **3D-Printing Filament (PLA)** | Material usage share for 3D printing enclosure and rear cover | 1 | $4.06 | $4.06 | Adafruit | [Adafruit #3728](https://www.adafruit.com/product/3728) |
| **Display Module (0.96" OLED)** | Fits into top surface recessed screen opening | 1 | $3.50 | $3.50 | Adafruit | [Adafruit #938](https://www.adafruit.com/product/938) |
| **Push Buttons (Tactile 6mm, 4-pack)** | Fit into control button wells | 1 | $3.50 | $3.50 | Adafruit | [Adafruit #367](https://www.adafruit.com/product/367) |
| **Speaker (8Ω 1W Mini Oval)** | Mounts behind rear acoustic speaker grille | 1 | $1.95 | $1.95 | Adafruit | [Adafruit #4227](https://www.adafruit.com/product/4227) |
| **USB Connector (Type-C Breakout)** | Slides into side panel USB cutout | 1 | $3.95 | $3.95 | Adafruit | [Adafruit #5180](https://www.adafruit.com/product/5180) |
| **LED Lighting (WS2812B 8-LED Stick)** | Installs into carved perimeter lighting channel | 1 | $4.95 | $4.95 | Adafruit | [Adafruit #1426](https://www.adafruit.com/product/1426) |

---

## Future Steps

While the CAD enclosure currently represents the physical exterior shell and static layout, the next phase of the project transitions into real-world hardware integration:

### LED Integration
Wiring WS2812B RGB LED strip hardware into the carved front groove.

### Acoustics & Sound
Soldering a physical mini speaker behind the rear acoustic vent grid.

### Microcontroller Integration
Mounting an ESP32 or Arduino microcontroller onto the internal corner posts.

### Software Coding
Writing firmware to bring the digital time display, alarms, and lighting effects to life.

---

## Latest Update: LED Display & Enclosure Integration
* **Display Recess:** Modeled and cut a precise, centered shallow recess into the top surface of the alarm clock enclosure in Onshape to securely house the digital display module.
* **LED Light Channel:** Added a concentric perimeter channel surrounding the display recess to embed and route the flashing alarm LED strip.
* **UI & Material Styling:** Designed a dedicated black screen panel complete with time, date, and alarm/music icons, alongside a translucent purple LED lighting effect.
* **Clearance Verification:** Validated structural alignment against the top-panel control buttons to ensure no enclosure intersections or hardware interference.


