# 🔬 Reproduction Guide: Step-by-Step Protocol

This document provides detailed instructions to reproduce the results reported in the manuscript *"Latency-Aware Service Function Chaining for Secure IoT Communications in SDN/NFV-enabled 5G Edge-Cloud Networks"*.

Following this guide should enable independent verification of all claims within **<30 minutes** on a standard laptop.

---

## 📋 Prerequisites

### Hardware Requirements
- **CPU**: 4+ cores (Intel i5/Ryzen 5 or equivalent)
- **RAM**: 8+ GB
- **Storage**: 2+ GB free space
- **OS**: Linux/macOS/Windows 10+

### Software Requirements
```bash
# Python version
python --version  # Must be 3.8, 3.9, or 3.10

# Required packages (installed via requirements.txt)
pip install -r requirements.txt

# Optional: For MILP baseline (academic license required)
# Visit: https://www.gurobi.com/academia/academic-program-and-licenses/