# Epidemics in Orbit: Junk Accumulation Model (JAM)

This repository contains code, simulations, and supporting materials for the paper:

**“Epidemics in Orbit: Modeling Space Debris Dynamics to Alleviate the Orbital Traffic Jam”**

---

## 🚀 Overview

The accumulation of space debris in Low Earth Orbit (LEO) poses a growing threat to satellite infrastructure, human spaceflight, and future missions.

This project introduces the **Junk Accumulation Model (JAM)**—a novel adaptation of the classical **SIR (Susceptible–Infectious–Removed)** epidemiological framework-to model space debris dynamics.

- **S (Susceptible):** Intact satellites and objects that can be hit  
- **I (Infectious):** Debris fragments capable of causing collisions  
- **R (Removed):** Objects removed via decay, burn-up, or active debris removal (ADR)  

JAM provides a **tractable, interpretable framework** to:
- Model debris proliferation
- Identify cascade thresholds (Kessler Syndrome)
- Evaluate mitigation strategies like ADR

---

## 🧠 Model Formulation

The JAM model is governed by the system of ODEs:
- dS/dt = Λ − βSI − μₛS
- dI/dt = (1 + θ)βSI − (γ + μᵢ)I
- dR/dt = γI + μₛS + μᵢI

Where:
- Λ = launch rate  
- β = collision rate  
- θ = debris generated per collision  
- γ = active debris removal (ADR) rate  
- μₛ, μᵢ = decay rates  

---

## 📊 Key Insights

- Debris behaves like an **epidemic system** with cascading growth dynamics  
- A reproduction number (R₀ / Rₑ) determines orbital stability  
- Without intervention → **runaway debris growth (Kessler Syndrome)**  
- Sustained ADR (~5%+) can suppress debris proliferation  

⚠️ This repository is part of academic research and is intended for exploratory and educational purposes.

---
## 🌐 Interactive Tool

An interactive JAM simulation tool (and underlying code) is available:
👉 **Interactive JAM tool:** https://jam-simulation.streamlit.app
🔗 **Underlying Code:** https://github.com/Rachel-Sholder/JAM-Streamlit

---

## 📁 Repository Structure

- **01 Simulation Code:** Core JAM implementation and reproduction of paper visuals
- **02 Historical Consistency:** JAM simulation of historical data (see Appendix A)
- **03 Figures:** Historical data figures (see Appendix A)
- **Data:** Supporting datasets (CSV and PDF)

---

## 👩‍🚀 Author

Rachel Sholder, JHU Doctor of Engineering  
Johns Hopkins University Applied Physics Laboratory (JHU/APL) 

Doctoral research bridging:
**epidemiology × orbital debris dynamics**

---

## 📌 Citation

If you use this work, please cite:

> R. Sholder, “Epidemics in Orbit: Modeling Space Debris Dynamics to Alleviate the Orbital Traffic Jam,” IEEE Aerospace Conference, 2026.

---
