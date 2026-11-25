# 📡 Public-Data Ground-Station Dashboard & Student Guide

An interactive ground-station pass-monitoring dashboard I built in Google Colab using `Skyfield`, `Gradio`, `NumPy`, `Pandas`, and `Matplotlib` with legal public orbital data and a follow-along guide designed so another student can reproduce the workflow.

## ✨ Key Features
- **Ground-Station Setup:** Configure station name, latitude, longitude, elevation, minimum elevation mask (degrees), and forecast window (hours).
- **Pass Window Calculation (AOS / LOS):** Computes satellite visibility windows, pass durations (minutes), and peak elevation angles using `Skyfield`.
- **Elevation & Pass Charts:** Displays an elevation-angle timeline relative to the station horizon mask alongside peak elevation bars per detected pass.
- **Follow-Along Student Guide & Pass Table:** Includes a clear step-by-step guide for students and a full-width pass schedule table in UTC.

## 🛠️ Tech Stack
- **Environment:** Google Colab
- **Orbital Propagation, Plotting & UI:** Python, `Skyfield`, `Gradio`, `NumPy`, `Pandas`, `Matplotlib`

## ⚙️ How to Run the Project
1. **Open in Google Colab:**
   - Upload the notebook or script to Google Colab (`colab.research.google.com`).
2. **Run & Launch:**
   - Run the cell to install `skyfield`, `gradio`, `numpy`, `pandas`, and `matplotlib` and launch the dashboard.
3. **Follow the Student Guide:**
   - Paste public TLE data (or load the sample public TLE block), enter your ground-station coordinates and elevation mask, and click **Build Ground-Station Dashboard**.

## 📌 Scope & Assumptions
- Uses lawful, publicly available orbital elements (TLE) and geometric line-of-sight/elevation calculations for educational pass planning; does not perform or encourage unauthorized RF reception or decryption.
- Pass predictions depend on TLE epoch freshness and assume unobstructed horizon beyond the configured minimum elevation angle.
