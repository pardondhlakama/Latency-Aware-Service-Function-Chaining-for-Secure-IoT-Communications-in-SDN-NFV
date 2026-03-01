# Latency-Aware Service Function Chaining for Secure IoT Communications

> **Manuscript**: "Latency-Aware Service Function Chaining for Secure IoT Communications in SDN/NFV-enabled 5G Edge-Cloud Networks"  
> **Author**: Pardon Taonaishe Dhlakama  
> **Course**: MNE503 Research Project  
> **Journal**: Submitted to MDPI Sensors, March 2026  
> **DOI**: [Will be assigned upon publication]  


[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/)
[![Reproducibility](https://img.shields.io/badge/reproducibility-100%25-brightgreen)](docs/reproduction_steps.md)

Overview

This repository contains the complete simulation framework for the latency-aware Service Function Chaining (SFC) orchestration framework described in the accompanying manuscript. The code implements:

-  Multi-objective optimization model (latency + security co-optimization)
- Two-phase heuristic algorithm (polynomial-time complexity)
-  SDN/NFV-enabled 5G edge-cloud network topology generator
-  Three baseline comparisons: Latency-Agnostic (LA), Security-First (SF), MILP-Exact (ME)
-  Statistical evaluation framework (95% confidence intervals, Student's t-test)

 Quick Start (Reproduce in <5 Minutes)

```bash
1. Clone repository
git clone https://github.com/pardondhlakama/Latency-Aware-Service-Function-Chaining-for-Secure-IoT-Communications-in-SDN-NFV.git
cd Latency-Aware-Service-Function-Chaining-for-Secure-IoT-Communications-in-SDN-NFV
 2. Create virtual environment (recommended)
python -m venv venv
source venv/bin/activate  # Linux/Mac
 OR for Windows:
 venv\Scripts\activate

 3. Install dependencies
pip install -r requirements.txt

 4. Run default simulation (small scale for testing)
python simulator/main.py --config config/small_scale.yaml

 5. Generate manuscript figures
python analysis/plot_results.py --input results/raw/ --output results/figures/
