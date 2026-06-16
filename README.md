# Part 1: Data Audit, EDA & Business Understanding

##  Overview
This part focuses on understanding the data, identifying quality issues, and extracting business insights from the D2C customer churn dataset.

##  Objectives
- Perform comprehensive data quality audit
- Identify missing values and data quality issues
- Analyze churn patterns and customer behavior
- Extract actionable business insights

## 📁 Files in This Part
part1-data-audit/
├── data_audit.ipynb # Complete EDA notebook
├── README.md # This file
├── churn_analysis.png # Churn visualizations
├── ticket_churn_analysis.png # Support ticket impact
└── web_activity_analysis.png # Web behavior analysis



### Data Quality Issues
| Issue | Count | Percentage |
|-------|-------|------------|
| Missing `loyalty_tier` | 1,386 | 57.8% |
| Missing `skin_type` | 401 | 16.7% |
| Orders with `_DUP` suffix | 1 | - |
| Outlier order values (>₹10,000) | 3 | - |
| Missing ratings | 80 | 3.3% |

### Churn Analysis Results
- **Overall Churn Rate**: 42.7%
- **Train Set Churn**: 42.9%
- **Validation Set Churn**: 41.7%
- **Test Set Churn**: 42.2%

### Key Business Insights
1. **Support Impact**: Customers with tickets churn at 58.3% vs 28.1% without tickets (2.1x higher)
2. **Ticket Volume**: Customers with 3+ tickets have 72.4% churn rate
3. **Sentiment**: Churned customers had 0.24 lower average sentiment score
4. **Recency**: Churned customers last visited 42.7 days ago vs 12.4 days for retained
5. **Best Channel**: Organic (18.2% churn)
6. **Worst Channel**: Instagram (52.8% churn)
