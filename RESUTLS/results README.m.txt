#  Results Documentation

This folder contains all empirical results supporting the claims in the manuscript *"Latency-Aware Service Function Chaining for Secure IoT Communications in SDN/NFV-enabled 5G Edge-Cloud Networks"*.

## Folder Structure

# Full-scale evaluation (30 runs, ~30 minutes)
python simulator/main.py --config config/default.yaml --runs 30 --algorithm proposed

# Quick test (5 runs, ~2 minutes)
python simulator/main.py --config config/small_scale.yaml --runs 5 --algorithm proposed
python analysis/plot_results.py --input results/raw/ --output results/figures/


## 🔄 How to Regenerate Results

### Prerequisites
```bash
# From repository root:
python -m venv venv
source venv/bin/activate  # Linux/Mac
# OR: venv\Scripts\activate  # Windows
pip install -r requirements.txt

python analysis/statistical_tests.py --data results/raw/ --output results/stats/