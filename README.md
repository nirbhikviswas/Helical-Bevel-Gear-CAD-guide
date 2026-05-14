# Helical Bevel Gear — Complete Manufacturing & CAD Guide ⚙️

[![Live Guide](https://img.shields.io/badge/View_Live_Guide-HTML-blue?style=for-the-badge)](https://nirbhikviswas.github.io/Helical-Bevel-Gear-CAD-guide/)
[![SolidWorks](https://img.shields.io/badge/SolidWorks-Compatible-red?style=for-the-badge)](#)
[![Engineering](https://img.shields.io/badge/Mathematics-Gleason_Standard-success?style=for-the-badge)](#)

A complete, self-contained mathematical reference and CAD workflow for designing and modelling a **properly-meshing** helical bevel gear pair. 

##  The Problem with Most Tutorials
If you search for "how to make a spiral bevel gear in SolidWorks," most tutorials teach a flawed method: applying a constant helix or a random twist angle along a cone. **This does not work.** Because a bevel gear's radius grows continuously from toe to heel, a constant-angle helix creates a tooth that fails to converge at the apex. The result? Gears that intersect, bind, and cannot mesh in the real world.

## 💡 The Solution
This guide uses proper mathematical integration based on Gleason standards to calculate the exact spiral curves, involute profiles, and taper laws required for true conjugate action. 

Every formula, Excel integration step, and SolidWorks click is documented.

##  What's Inside

This repository contains a single, highly-detailed HTML guide that breaks down the entire process:

1. **Geometry Fundamentals:** Understanding the apex, cone distance, and virtual tooth counts.
2. **The Mathematics:** Calculating pitch cone angles, cone distances, tooth height tapers, and the involute profile.
3. **Angular Integration:** Why the spiral angle ($\beta$) must vary, and the numerical integration required to plot it:
   $$\Delta\phi_i = \frac{\tan(\beta_{avg})}{R_{avg}} \Delta t$$
4. **Excel Setup:** A row-by-row guide to building the 50-point coordinate tables ($X, Y, Z$) for the centreline, tip, and root curves.
5. **SolidWorks Workflow:** Step-by-step instructions for importing the XYZ curves, creating the variable section sweep, and using guide curves to enforce the linear taper law.
6. **Assembly & Verification:** How to correctly mate the left-hand pinion and right-hand gear to verify the 1:1 mesh.

###  Base Example Parameters
The guide walks through a complete example with the following specifications:
* **Ratio:** 1:1
* **Teeth ($N$):** 20
* **Module at mean ($m$):** 3 mm
* **Spiral Angle ($\beta$):** 35°
* **Pitch Cone Angle ($\Gamma$):** 45°
* **Face Width ($F$):** 20 mm

## 🛠️ How to Use This Repo

1. **Read the Guide:** Click the [Live Guide](#) link at the top of this README to open the interactive HTML page.
2. **Download the Data:** Use the export buttons within the HTML guide to download the pre-calculated `pinion_spiral.txt` and `gear_spiral.txt` XYZ coordinate files.
3. **Follow the CAD Steps:** Open SolidWorks and follow **Part 4** of the guide to import the curves and generate the true gear geometry.

##  Author
**Nirbhik Viswas** Mechanical Engineering & Design
