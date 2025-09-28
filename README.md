# 🔬 Spectrometer Optimal Slit Width Calculator & Infographic

An interactive, single-page web application (SPA) designed to visualize and calculate the **Optimal Entrance Slit Width ($w$)** for a custom-built VIS-NIR Spectrometer. This project accompanies **Part 8** of the JAPSER Spectrometer design series.

The optimal slit width is crucial for balancing **spectral resolution** (the ability to distinguish close wavelengths) with **optical throughput** (the amount of light entering the system).

## 🎯 Core Concept & Formula

This tool implements the final derived equation for the optimal slit width in an infinity-corrected spectrometer setup. The equation is critical because it links the desired spectral resolution ($\Delta\lambda$) directly to the physical design parameters of the system.

The application calculates the slit width ($w$) in micrometers ($\mu m$) using the following formula:

$$
w = \frac{m \cdot \Delta\lambda \cdot L_C}{d \cdot \cos(\beta)}
$$

### Parameters:

| Symbol | Description | Unit in Calculator | 
| ----- | ----- | ----- | 
| $w$ | Optimal Slit Width | $\mu m$ (Calculated) | 
| $m$ | Diffraction Order | (Unitless) | 
| $\Delta\lambda$ | Target Spectral Resolution | $nm$ | 
| $L_C$ | Collimating Lens Focal Length | $mm$ | 
| $d$ | Grating Groove Spacing ($1/Grooves$) | $nm$ (Derived from input) | 
| $\beta$ | Diffraction Angle for $\lambda_{min}$ | $degrees$ | 

## ✨ Features

1. **Interactive Calculator:** Real-time calculation of the optimal slit width as input parameters are adjusted.

2. **Infographic Format:** Step-by-step visual explanation of the physical and geometric principles behind the final derivation.

3. **Sensitivity Analysis:** A **Chart.js** visualization demonstrating how a change in each input parameter (e.g., $L_C$ or $\Delta\lambda$) affects the resulting slit width, providing instant design insight.

4. **Single-File SPA:** The entire application is contained within a single `index.html` file for easy deployment.

## ⚙️ Technology Stack

| Technology | Purpose | 
| ----- | ----- | 
| **HTML5** | Core structure and content. | 
| **Tailwind CSS (CDN)** | Fully responsive layout and modern UI/UX design. | 
| **Chart.js (CDN)** | Rendering the interactive parameter sensitivity bar chart. | 
| **Pure JavaScript** | Handling input, formula calculation, and DOM manipulation. | 

## 🚀 Usage

### Accessing the Live Demo

You can view the live, hosted version of the calculator using [GitHub Pages](https://pages.github.com/):

> **https://checkag.github.io/Jasper_VIS_NIR_Slit_Width/**

### Running Locally

Since the application is a single HTML file with no build steps or server requirements, you can run it instantly:

1. Clone this repository:
   
git clone https://github.com/checkag/Jasper_VIS_NIR_Slit_Width.git

2. Open the `index.html` file in any web browser.

## 🤝 Contribution

This project is a component of a larger open-source spectrometer build. Feedback, bug reports, and suggestions for formula improvements or additional features are welcome!
