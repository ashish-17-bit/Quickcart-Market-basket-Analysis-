QuickCart Market Basket Analysis
​A comprehensive Python-based Market Basket Analysis and Association Rule Mining project for QuickCart retail stores. This project processes customer transaction data to discover frequent item purchasing patterns, cross-selling opportunities, and product affinities using standard machine learning and data mining algorithms.
​🚀 Project Overview
​Market Basket Analysis (MBA) helps retailers understand customer purchasing behavior by uncovering associations between items. Using transaction logs from QuickCart stores, this notebook builds a binary one-hot encoded matrix of customer baskets and applies association rule mining algorithms to extract actionable insights.
​Key Capabilities:
​Transaction Processing: Transforms long-format transaction logs into basket-level lists and binary one-hot matrices using mlxtend's TransactionEncoder.
​Frequent Itemset Mining: Benchmarks and extracts frequent itemsets using both Apriori and FP-Growth algorithms with configurable minimum support thresholds (min_support=0.02).
​Association Rule Generation: Computes metrics such as Support, Confidence, and Lift to evaluate product relationships.
​Planted Pattern Verification: Validates mined rules against 6 predefined ground-truth retail product pairings.
​📁 Project Structure & File Manifest
​Quickchart_Basket.ipynb: Main Jupyter Notebook containing the data loading, preprocessing, mining, and verification workflow.
​quickcart_basket_transactions.csv: Core transaction log containing line items, order IDs, dates, store IDs, SKU IDs, SKU names, and categories (26,878 line items across 5,000 unique baskets/orders).
​dim_skus.csv: Product catalog mapping SKU IDs to names and categories (60 unique products/SKUs).
​frequent_itemsets.csv: Pre-computed or generated frequent itemsets from the mining process.
​association_rules_full.csv: Full set of generated association rules detailing antecedents, consequents, support, confidence, and lift.
