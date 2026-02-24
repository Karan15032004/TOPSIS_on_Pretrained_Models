# Applying TOPSIS to Select the Best Pre-trained Model for Text Summarization

# Project Overview

This project applies the TOPSIS (Technique for Order Preference by Similarity to Ideal Solution) method to identify the best pre-trained model for Text Summarization.
Instead of selecting a model based on a single metric, this project evaluates multiple performance and efficiency criteria simultaneously and ranks the models using multi-criteria decision-making.


# Objective

The goal of this assignment is to:
- Select multiple pre-trained text summarization models
- Define evaluation criteria (performance + efficiency)
- Construct a decision matrix
- Apply the TOPSIS algorithm
- Rank the models
- Identify the best model


# Models Evaluated

The following widely-used pre-trained models were considered:

- BART-large-CNN
- T5-base
- Pegasus-XSum
- DistilBART
- LED-base


# Evaluation Criteria

The models were evaluated using both performance-based and cost-based metrics.

# Benefit Criteria (Higher is Better)
- ROUGE-1
- ROUGE-2
- ROUGE-L

These measure summarization quality.

# Cost Criteria (Lower is Better)

- Inference Time (seconds)
- Model Size (MB)

These measure computational efficiency.


# Decision Matrix

A structured decision matrix was created using benchmark-style performance values.
Each row represents a model, and each column represents a criterion.


# Methodology

The following steps were used to apply TOPSIS:

# Step 1: Normalize the Decision Matrix
Vector normalization was applied to remove scale differences.

# Step 2: Apply Weights
Weights were assigned to each criterion to reflect importance.

# Step 3: Determine Ideal Best and Ideal Worst
Ideal Best: Maximum benefit values and minimum cost values
Ideal Worst: Minimum benefit values and maximum cost values

# Step 4: Compute Separation Measures
Distance from ideal best and ideal worst was calculated.

# Step 5: Compute Closeness Coefficient
The TOPSIS score (closeness coefficient) was computed for each model.

# Step 6: Rank the Models
Models were ranked based on descending TOPSIS score.


# Results

- A ranking table was generated.
- A bar graph visualized the TOPSIS scores.
- The model with the highest closeness coefficient was selected as the best model.

The ranking reflects a balance between summarization performance and computational efficiency.



# Visualization

A bar chart was generated to compare:

- Model names
- Corresponding TOPSIS scores

The highest bar indicates the best-performing model according to the multi-criteria analysis.



# Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
