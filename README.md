# Fuzzy Smart Waste-Sorting Control System (FSWSCS)

This repository is the code for the python implementation for assignment 1 of _CSC3034 Computational Intelligence_,

Focusing on the Sustainable Development Goals (SDG) 11 and 12, This is an intelligent fuzzy logic–based decision system designed to classify common waste materials into the following:

1. paper
2. organic
3. plastic
4. metal

Unlike rigid threshold-based classifiers, FSWSCS handles uncertainty in sensor data (e.g., dirt, moisture, mixed materials) through fuzzy reasoning, producing smoother and more human-like decisions.

## System Workflow

The overall architecture follows the standard fuzzy control pipeline:

Inputs → Fuzzifier → Rule Base & Inference Engine → Defuzzifier → Output

## 📊 Example Use Case

| Case | Reflectivity | Moisture | Weight | Magnetic | Predicted |
| ---- | ------------ | -------- | ------ | -------- | --------- |
| 1    | 0.85         | 0.10     | 0.25   | 0.00     | Plastic   |
| 2    | 0.40         | 0.65     | 0.45   | 0.05     | Organic   |
| 3    | 0.20         | 0.25     | 0.35   | 0.90     | Metal     |
| 4    | 0.35         | 0.20     | 0.25   | 0.10     | Paper     |

---

## 🧩 Dependencies

- Python 3.8+
- NumPy
- scikit-fuzzy
- matplotlib

Install with:

```bash
pip install numpy scikit-fuzzy matplotlib
```
