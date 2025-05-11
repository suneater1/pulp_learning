# 🐱 Whiskas Blending Optimization (Linear Programming in Python)

This project solves a **blending optimization problem** using linear programming with [PuLP](https://coin-or.github.io/pulp/). The goal is to create the cheapest possible 100g can of Whiskas-style cat food while meeting specific **nutritional requirements**.

## 📦 Problem Overview

We aim to determine the ideal amounts (in grams) of each ingredient to include in a 100g can of cat food. Each ingredient has:
- A cost per gram
- Nutritional contributions (protein, fat, fiber, salt)

### 🔍 Objective
Minimize the **total cost** of ingredients per can while satisfying:
- **Protein ≥ 8g**
- **Fat ≥ 6g**
- **Fibre ≤ 2g**
- **Salt ≤ 0.4g**

## 🛠 Tools Used

- Python
- [PuLP](https://pypi.org/project/PuLP/) – Linear programming modeling
- `pandas` for data handling
- `matplotlib` + `squarify` for visualization
- `jupyter` for interactive development

## 📁 Project Structure

```plaintext
├── data/
│   ├── ingredients.csv        # Cost and nutrition data per ingredient
│   └── constraints.csv        # Nutritional requirements (min/max)
├── whiskas_blending.ipynb     # Main notebook (formulation + results)
├── requirements.txt           # Required Python packages
├── results/
│   ├── solution_plot.png      # Bar chart of ingredient blend
│   └── solution_treemap.png   # Treemap of composition (optional)
├── LICENSE                    # License (public domain dedication)
└── README.md                  # This file
