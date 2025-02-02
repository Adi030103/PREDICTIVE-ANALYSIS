# PREDICTIVE-ANALYSIS
Assignment-3(Topsis to find best pre-trained model for text sentence similarity)
# Description

This Python script applies the **TOPSIS (Technique for Order Preference by Similarity to Ideal Solution)** method to rank **pretrained sentence similarity models** (BERT, RoBERTa, SBERT, GPT, and T5) based on multiple evaluation criteria. 

Key Steps:
1. Define the Decision Matrix  
   - The models are evaluated on STS-B (Semantic Textual Similarity Benchmark) using metrics:  
     - Cosine Similarity, Pearson Correlation, Spearman Correlation (higher is better)  
     - Inference Time, Memory Usage (lower is better)  

2. Normalize the Decision Matrix 
   - Converts all values into a comparable scale.  

3. Assign Weights  
   - More importance is given to similarity metrics, while inference time and memory usage have lower weights.  

4. Compute Ideal Best and Worst Values  
   - Identifies the best and worst performance for each criterion.  

5. Calculate Euclidean Distances  
   - Measures the distance of each model from the ideal best and worst solutions.  

6. Compute TOPSIS Scores & Rank Models  
   - The model with the highest score is the best choice.  

7. Visualize Results  
   - The script prints the ranked models and generates a bar chart using Seaborn to illustrate the rankings.  

# Outcome:
Based on the TOPSIS analysis, GPT emerged as the best model for text sentence similarity. Despite having a higher inference time and memory usage, its similarity metrics (Cosine, Pearson, and Spearman correlations) contributed to its top ranking. This indicates that GPT excels in capturing nuanced sentence relationships, making it a strong choice for applications requiring high-quality semantic similarity detection. 
