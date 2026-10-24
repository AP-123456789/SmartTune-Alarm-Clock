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

| No. | Item | Quantity | Purpose |
| :--- | :--- | :--- | :--- |
| 1 | Main enclosure | 1 | Outer body of the alarm clock |
| 2 | Rear cover | 1 | Covers the back of the enclosure |
| 3 | Screws | 4 (proposed) | Secure the rear cover |
| 4 | 3D-printing filament (PLA) | As required | Material for printing the enclosure and cover |
| 5 | Display module | 1 (proposed) | Fits into the display opening |
| 6 | Push buttons | 4 (proposed) | Fit into the button openings |
| 7 | Speaker | 1 (proposed) | Fits behind the speaker grille |
| 8 | USB connector/module | 1 (proposed) | Fits into the USB opening |
| 9 | LED lighting | As required (proposed) | Provides the planned lighting effect |

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

---

## Project Viewable Design (Onshape)

https://cad.onshape.com/documents/89b7b359616dac68ca74ce6f/w/914e3c94c6e810e6c0479be0/e/4a201dfb63b84187a3f467ad?renderMode=0&uiState=6add22c75837a283378819b2

