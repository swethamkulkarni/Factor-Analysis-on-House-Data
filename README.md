# Factor Analysis on King County House Data

Identified latent variables in KC house data using Factor Analysis. Part of my ML coursework.

## What I did

Took 5 property features (condition, grade, above-ground footage, basement footage, living area) and ran factor analysis to see what underlying patterns existed. Standardized the data and fitted a 2-component model to uncover the hidden factors driving house characteristics.

## Results

Found two meaningful factors:

**Quality** - Driven by grade, above-ground space, and living area. Houses with better construction and more above-ground footage load heavily on this factor.

**Size** - Primarily determined by basement square footage. Larger basements define this dimension, while better-grade houses actually load negatively, suggesting size and quality are somewhat independent.

KMO score of 0.672 indicates moderate suitability for factor analysis, meaning the data was reasonably suited for this approach.

## Tech

Python, Scikit-learn, Pandas, NumPy, factor_analyzer

## Run it

Install dependencies:
```bash
pip install pandas numpy scikit-learn factor-analyzer
```

Run the notebook:
```bash
jupyter notebook sub_task_3.ipynb
```

You'll need `kc_house_data_reduced.csv` in the same directory.

## Key takeaway

Factor analysis reduced 5 correlated variables into 2 interpretable latent factors, making it easier to understand what really drives differences in house characteristics without relying on price.
