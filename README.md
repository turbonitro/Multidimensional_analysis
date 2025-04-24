# Multidimensional_analysis
Multidimensional analysis - Polish political scene / The wildest voivodeship in Poland

This repository contains two multivariate analysis projects, which attempt to answer the question of which voivodeship in Poland is the least socially and infrastruturally violated, and which politician from the analyzed actors of the Polish political scene comes closest to the ideal politician.

______________________________________________________________________________________________

1. Identifying Poland's Wildest Regions for Off-Grid Living

This project analyzes the impact of human activity on Poland's natural landscapes to identify the least human-affected regions, ideal for off-grid living. Motivated by research highlighting the negative effects of urbanization on mental and physical health (e.g., Alok & Sunil, 2015; Corey, 2013), and the growing desire for nature connection (Neale & Stroud, 2019), the study explores whether remote work and technological advancements (e.g., Starlink, renewable energy) make living in pristine areas feasible. The analysis uses statistical methods to rank Polish voivodeships based on their "wildness," leveraging data from the Central Statistical Office (GUS).
Key Features:
Dataset: 17 environmental and human-impact variables (e.g., forest area, population density, pollution levels) from GUS, with 15 destimulants (negative impact) and 2 stimulants (positive impact). Variable X17 (vehicles per capita) was excluded due to low variability (<10%).

Linear Ordering Methods:
Pattern Method (with/without weights), TOPSIS, and Rank Sum Method rank voivodeships by minimal human interference.

Top regions: Podkarpackie, Lubuskie, Podlaskie, Pomorskie, Warmińsko-Mazurskie.

Śląskie consistently ranks lowest due to high urbanization and industrial activity.

Principal Component Analysis (PCA):
Four principal components explain 84.92% of variance, driven by variables like population density (X4), building area (X5), railway length (X7), and wild landfill area (X14).

Variables X8 (water consumption) and X10 (protected areas) were excluded due to low correlation.

Visualizations (e.g., factor plane projections, Chernoff faces) highlight Śląskie’s industrial dominance and the natural integrity of top-ranked voivodeships.

Cluster Analysis:
Hierarchical clustering (Ward’s method, average linkage) groups similar voivodeships, confirming a cluster of low-impact regions (Podkarpackie, Lubuskie, Podlaskie, Pomorskie, Wielkopolskie).

Key Observations:
Podkarpackie emerges as the top candidate for pristine landscapes, though differences among top voivodeships are subtle.

Śląskie is the most human-altered region, driven by urban and industrial factors.

Anomalous water consumption in Świętokrzyskie (10x higher than Śląskie) warrants further investigation.

Tools:
Statistica

Data Source:
Central Statistical Office (GUS), accessed February 2023.

______________________________________________________________________________________________

2. Analysis of Preferred Traits in an Ideal Polish Politician

The study aims to identify the traits preferred in an ideal Polish politician and compare these with perceptions of real Polish politicians. Using a survey of 202 respondents, the analysis evaluates preferences across demographic groups and conducts a detailed correspondence analysis of empathy and politeness for two politicians: Władysław Kosiniak-Kamysz and Paweł Kukiz. The project leverages statistical methods to explore public perceptions of politicians and the Polish political landscape.
Key Features:
Dataset:
Survey Structure: 202 respondents answered questions in three parts:
Demographics: Age (6-level ordinal), gender (binary nominal), education (4-level ordinal).

Politician Evaluations: 9 politicians (including an "ideal" politician) rated on 18 traits (e.g., honesty, empathy, conservatism) on a 1–100 interval scale.

Political Scene Opinions: 20 statements about Polish politics rated on a 7-point Likert scale (ordinal).

Respondent Profile: Predominantly young adults (48% aged 20–29) and highly educated (58% with higher education), potentially skewing representativeness compared to Poland’s population (e.g., only 23.1% nationally have higher education).

Descriptive Analysis:
Ideal Politician Traits: Responsibility, honesty, and engagement are most valued; "troublemaking" (mąciwoda) and conservatism are least desired.

Politician Rankings: Rafał Trzaskowski and Szymon Hołownia score closest to the ideal politician, while Przemysław Czarnek, Paweł Kukiz, Zbigniew Ziobro, and Janusz Korwin-Mikke score lowest.

Polish Political Scene: Respondents view Polish politicians negatively, citing broken promises (mean: 2.77), corruption (mean: 5.08), societal polarization (mean: 5.95), and nepotism (mean: 5.27). They support abolishing parliamentary immunity (mean: 4.89) and reducing politicians’ salaries (mean: 5.18).

Correspondence Analysis:
Kosiniak-Kamysz and Kukiz: Focused on empathy and politeness (converted to nominal categories: empathetic/non-empathetic, polite/impolite).
Both received similar ratings: ~40% rated as polite-empathetic, ~32% as impolite-non-empathetic, across age and education groups.

Low quality (0.24) for Kosiniak-Kamysz’s "impolite-empathetic" category suggests poor representation.

No clear trait associations for Kosiniak-Kamysz; for Kukiz, polite-non-empathetic and impolite-empathetic are linked.

Age groups 20–29, 30–39, and 60–69 show similar profiles; respondents aged 70+ and those with primary education are outliers.

All Politicians: Two dimensions explain ~87% of inertia.
Trzaskowski, Hołownia, and Kosiniak-Kamysz are closest to the ideal politician, associated with responsibility, politeness, and honesty.

Korwin-Mikke, Ziobro, Czarnek, and Kukiz are furthest, linked to conservatism and troublemaking.

Chernoff faces and clustering confirm two politician groups: (1) Trzaskowski, Hołownia, Kosiniak-Kamysz, Biedroń; (2) Korwin-Mikke, Ziobro, Czarnek, Kukiz. The ideal politician remains distinct.

Factor Analysis:
Purpose: Consolidate 20 political scene questions into latent factors.

KMO and Bartlett’s Test: KMO = 0.800 (adequate sample); Bartlett’s test (χ² = 1018.611, p < 0.000) rejects sphericity, supporting factor analysis.

Principal Components: 5 factors (eigenvalues > 1) explain ~55% of variance; 3 factors retained after Quartimax rotation for clarity:
Factor 1: International Engagement (~20.8% variance): Questions on international representation, climate action, and pandemic response (e.g., Q8, Q18, Q19). Respondents view Polish politicians’ international performance poorly.

Factor 2: Political Ethics (~12.3% variance): Questions on immunity, salaries, polarization, and nepotism (e.g., Q10, Q11, Q12, Q14). Negative perceptions dominate.

Factor 3: Political Awareness (~9.2% variance): Focuses on voter political awareness (Q17), rated low by respondents.

Demographic Variations:
Gender: Men value mediality and conservatism more than women.

Education: Respondents with primary education prioritize openness, empathy, conservatism, and education.

Age: Conservatism is most valued by those 70+; troublemaking is least bothersome to 30–39-year-olds but disliked by 60–69-year-olds.

Tools:
Excel: Descriptive statistics, tables, and visualizations (e.g., box plots, Chernoff faces).

Statistica: Correspondence analysis, factor analysis, and principal component analysis.

Applications:
Provides insights into public expectations for politicians, useful for political campaigns and policy design.

Highlights gaps between ideal and actual politicians, informing voter education and political reform.

Identifies public discontent with Poland’s political scene, relevant for addressing corruption, polarization, and gender inequality.

Limitations:
Sample bias (overrepresentation of young, highly educated respondents) may limit generalizability.

Low quality scores for some correspondence analysis categories (e.g., Kosiniak-Kamysz’s impolite-empathetic) suggest potential misrepresentation.

Factor analysis explains only ~55% of variance, indicating other unmeasured factors may influence perceptions.

Conclusions:
Ideal Politician: Characterized by responsibility, honesty, and engagement; Trzaskowski and Hołownia align closest, while Korwin-Mikke and Ziobro are furthest.

Kosiniak-Kamysz and Kukiz: Similar empathy and politeness ratings, but no strong trait associations; demographic variations (age, education) influence perceptions.

Political Scene: Negative public sentiment toward Polish politics, with concerns about corruption, polarization, and poor international performance.

Recommendations: Future studies should use more representative samples and explore additional traits or factors to capture a fuller picture of public sentiment.

Tools:
Statistica

