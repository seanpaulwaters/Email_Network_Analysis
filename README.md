# Management Salary Prediction in Networks

## Overview
This project centers on predicting 'ManagementSalary' status within a company's email network. Using a dataset of internal email communications, it aims to determine which employees are likely on a management-level salary. The project uniquely combines network analysis with machine learning to solve this business challenge, offering insights into the role of network position in organizational hierarchy.

## Installation and Usage

### Dependencies
- Python 3.x
- Libraries: pandas, numpy, NetworkX, sklearn

### Setup
- Clone the repository to your local machine using `git clone [repository URL]`.
- Install the required dependencies by running `pip install -r requirements.txt` in your command line.

### Running the Project
- Navigate to the project's root directory.
- Open and run the Jupyter notebook `email-network-analysis.ipynb` to view the analysis.

## File Structure
- `email-network-analysis.ipynb`: The main Jupyter notebook containing the analysis and model training.
- `assets/`: Contains the graph data used in the project.
- `requirements.txt`: Lists all the Python dependencies required for the project.
- `README.md`: This file, providing an overview and guide for the project.

## Methodology
- **Data Exploration**: Analyzing the structure and attributes of the company's email network.
- **Network Analysis**: Applying network analysis techniques, such as centrality measures and community detection, to explore and visualize network characteristics.
- **Feature Engineering**: Developing features based on network attributes to predict management salary likelihood, focusing on both local and global network properties.
- **Predictive Modeling**: Implementing and training machine learning classifiers using scikit-learn.
- **Model Evaluation**: Assessing model performance using metrics like Area Under the Receiver Operating Characteristic Curve (AUC).

## Results and Discussion

### Model Performance
- Enhanced performance was observed in Random Forest and XGBoost models post hyperparameter tuning, with Random Forest marginally outperforming, demonstrating its effectiveness in complex network data analysis.

### Key Insights
- **Network Features' Predictive Power**: Centrality measures like Betweenness, Clustering, Closeness, and Degree were pivotal in predicting management salaries, highlighting the significance of an individual's network position.
- **Interpretability**: Insights into the influence of network attributes on management salary predictions were gained through feature importance rankings and Partial Dependence Plots.

### Implications
- **Organizational Dynamics**: The analysis provides valuable insights into network dynamics within an organization, potentially guiding structural analysis and optimization.
- **Talent Identification**: The correlation between network attributes and management roles offers a data-driven approach to identifying leadership potential.

### Limitations and Future Directions
- **Generalizability**: The models may best apply to organizations with similar communication networks, and further validation in diverse settings is recommended.
- **Data Diversity**: Incorporating a variety of data types could enhance predictive accuracy beyond the current reliance on email data.
- **Temporal Analysis**: Future research could focus on the evolution of network roles over time to inform leadership development strategies

## License

MIT License
