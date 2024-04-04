# Indiana COVID-19 Vaccination Geospatial Clusters

## Project Overview
This project leverages data analytics and machine learning techniques to identify patterns in COVID-19 vaccination rates across Indiana, with a focus on how these rates correlate with geographic locations. By applying Bayesian Gaussian Mixture Models (GMM) for clustering, we aim to uncover trends and disparities in vaccination rates, providing insights that can inform public health strategies.

## Objectives
- To analyze COVID-19 vaccination trends across Indiana's zip codes.
- To identify geographic correlations in vaccination rates using GMM clustering.
- To highlight disparities in vaccination rates, offering a foundation for targeted intervention strategies.

## Data Source
The dataset consists of COVID-19 vaccination data provided by the Indiana Department of Health, covering the years 2019 to 2022. Key data points include the number of vaccinations administered (first dose, fully vaccinated, booster doses), alongside demographic information based on ZIP code populations.

## Technical Details

### Data Preprocessing
Key preprocessing steps included:
- **Handling Missing Values**: Entries marked as "Suppressed" were estimated to protect individual privacy.
- **Normalization**: Adjusted data to account for population size differences across ZIP codes.
- **Principal Component Analysis (PCA)**: Reduced dataset dimensionality while preserving 99.92% of the variance.

### Gaussian Mixture Model (GMM) Clustering
- **Implementation**: Used Scikit-learn's `GaussianMixture` class to perform GMM clustering.
- **Model Selection**: Employed the Bayesian Information Criterion (BIC) to determine the optimal number of clusters.

### Model Evaluation
- **Silhouette Score**: Achieved a silhouette score of 0.54178, indicating well-defined clusters.

### Visualization
- **Tableau Dashboards**: Created to visualize geospatial clusters, enabling easy identification of vaccination trends across ZIP codes.

## Tools and Libraries
- **Python Libraries**: Utilized `pandas`, `numpy`, `matplotlib`, `seaborn`, and `scikit-learn` for data manipulation, analysis, and modeling.
- **Visualization**: Tableau was used for creating interactive dashboards to present our findings.

## Findings and Conclusion
Our analysis revealed significant disparities in vaccination rates across Indiana, with urban areas typically showing higher rates. The project underscores the importance of geospatial analysis in public health, offering a pathway to more targeted and effective vaccination strategies.

## References
This project references works such as "Mathematics for Machine Learning" by Deisenroth et al., "Machine Learning: A Probabilistic Perspective" by Murphy, and utilizes documentation from the Scikit-learn library for methodological guidance.

---

This README.md combines an overview of the project's goals and findings with detailed information on the methodologies, data preprocessing steps, and tools used, offering a complete picture suitable for GitHub viewers interested in both the project's impact and its technical underpinnings.
