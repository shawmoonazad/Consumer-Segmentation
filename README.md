# Segmenting consumers through unsupervised machine learning and the theory of planned behavior: Insights for digital commerce in Bangladesh

* This repository accompanies the work "Segmenting consumers through unsupervised machine learning and the theory of planned behavior: Insights for digital commerce in Bangladesh," published in *Computers in Human Behavior Reports* (Elsevier).
* Authors of the work: MD. Shahriar Bin Nazmul, Md Shawmoon Azad, M.R.C. Mahdy.
* Corresponding author: Dr. M.R.C. Mahdy.

### Idea

Most work applying the Theory of Planned Behavior to online consumer behavior treats attitude, subjective norms, and perceived behavioral control as predictors of a known outcome, usually through structural equation modeling or a supervised classifier. This study asks a different question. Instead of testing whether TPB constructs predict purchasing, it uses them as the coordinate system in which consumers are located, and lets an unsupervised algorithm find the groups.

Twelve TPB items serve as input features for K-means clustering on 266 Bangladeshi social-media users. The result is three psychologically interpretable segments rather than a predicted purchase outcome: Moderate Engagement, High Engagement, and Low Engagement/Resistant. Each segment is described in terms of how people actually behave on these platforms, whose opinions they consult, how far they trust unfamiliar sellers, and how capable they feel of completing a transaction.

The study is explicitly exploratory and descriptive. The clustering and the PCA projection are used to identify and visualize patterns, not to test causal hypotheses, and the findings are reported as segment-level associations rather than as causal evidence.

### Approach

* Reliability of the three TPB subscales is assessed with Cronbach's alpha before any clustering, so the features entering the model are known to be internally consistent.
* Cluster solutions are evaluated across four internal criteria (Elbow/WCSS, Silhouette, Davies-Bouldin, Calinski-Harabasz) for k = 2 through k = 8, rather than relying on the elbow method alone.
* One-way ANOVA with Tukey HSD post hoc tests describes separation between the retained clusters. Because the same constructs formed the clusters, these are reported as evidence of separation, not as independent validation.
* A Random Forest classifier trained on an 80% partition and stratified 10-fold cross-validation check whether the segment labels are recoverable beyond the full-sample solution.
* PCA is used only to render the cluster structure in two dimensions. It is not a preprocessing step and not an input to the clustering.

### Findings

* Three segments emerge: Moderate Engagement (56.8%), High Engagement (22.2%), and Low Engagement/Resistant (21.1%).
* Attitude carries the strongest endorsement across all clusters. Subjective norms and perceived behavioral control show high neutral-response rates, between 30% and 51% on many items, which points to a market where beliefs about safety and ease of transacting have not yet settled.
* Horizontal peer norms matter more than vertical family norms. Family influence records the lowest mean of any item, while peer encouragement and social validation characterize the High Engagement segment. This has implications for how TPB instruments developed in Western or East Asian settings transfer to South Asian digital markets.
* The segments map onto differentiated communication strategies: social proof and conversion-oriented engagement for the highly engaged, trust signals and informational content for the moderate group, and gradual low-pressure onboarding for the resistant group.

### Dataset

* Cognitive purchase behavior of Bangladeshi consumers on social media (Rahman et al., 2024)
* Website: https://data.mendeley.com/datasets/p5dgz597wn/1
* DOI: 10.17632/p5dgz597wn.1

This study is a secondary analysis of the de-identified, publicly available dataset above. No new data were collected. The original collection was carried out by the team that produced the dataset, under their own institutional protocol.

The dataset holds 266 completed questionnaires with 29 features covering demographics (age, gender, occupation, income), behavioral profile items, and TPB constructs measured on a five-point Likert scale. Only the twelve TPB items (ATTD1-ATTD4, SN1-SN4, PBC1-PBC4) are used as clustering inputs. The Purchase Behavior items and the demographic variables are used for descriptive interpretation only.

### Citation

Bin Nazmul, M. S., Azad, M. S., & Mahdy, M. R. C. (2026). Segmenting consumers through unsupervised machine learning and the theory of planned behavior: Insights for digital commerce in Bangladesh. *Computers in Human Behavior Reports*, 101237. https://doi.org/10.1016/j.chbr.2026.101237

### Contact

Md Shawmoon Azad: shawmoon.azad@northsouth.edu

Dr. M.R.C. Mahdy: mahdy.chowdhury@northsouth.edu
