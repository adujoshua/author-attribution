# author-attribution

--- Read Me----

This is a redacted version of a semester paper of a Masters program in Economics at the University of Kassel, Germany.

Topic: Comparative Analysis of Bibliometric weighting methods: A Case Study of University of Kassel and Klinikum Kassel

Coding was done in R markdown ( .rmd)
Relevant dataset - four csv files attached.
PowerPoint presentations (Author attribution.pdf) provide further insights and explanations
Name: Joshua Adu

Date: 19 January, 2026

linkedin: https://www.linkedin.com/in/adujoshua/

....Publication volumes and methods of co-author weighting...###
Publication volumes are among the key indicators in bibliometrics. However, simple counts (full counting) have methodological weaknesses, since publications are usually produced in teams and the number of contributing authors can vary greatly.

To address this problem, bibliometric research has developed several methods of co-author weighting:

#____ Weighting Methods ______

• Full Counting: Each participating institution receives a score of 1, irrespective of the number of authors contributed by the institution

• Fractional counting: Each publication is distributed equally across all contributing authors: Wi = 1/n. where is the number of authors. example: A publication with five authors contributes 0.2 to the publication volume of each. 1 publication with 4 authors → each receives 0.25.

• First-author weighting: The first author receives a larger share (e.g., 0.5), while the remaining share is distributed equally among the other authors. Example: The first author (i = 1) receives weight 𝑤1 = 0.5. The remaining n−1 authors (i = 2, … , n) share the other 0.5 equally: Wi= 0.5/(𝑛−1) for i= 2,…,n This ensures ∑ W𝑖 = 1

• Harmonic counting: Shares decrease harmonically with the author position. Weights are calculated according to where i is the author’s position and n is the total number of authors. Example: 1 publication with 3 authors. Raw weights: 1/1 (author 1), 1/2 (author 2), 1/3 (author 3). Sum = 1 + 0.5

0.333… = 1.833. Normalized weights: author 1 = 1 / 1.833 ≈ 0.545, author 2 = 0.5 / 1.833 ≈ 0.273, author 3 = 0.333 / 1.833 ≈ 0.182. Thus, the first author receives a substantially larger share, but other authors are not excluded.
•𝟏/√N-counting: Each contributing author receives 𝟏/√N. Therefor each institution receive [ (𝟏/√N) times Number of Authors from Institution]

#----- Objectives-------

In this project, I will examine how different weighting methods affect the measured publication volume of two institutions: the University of Kassel and Klinikum Kassel for 2023 publications. Main questions:

• Which method is preferred in a real bibliometric evaluation?

• Which factors (e.g., discipline, team size, authorship conventions) play a role in this decision?

• Which differences arise between the methods?

• I will also model with hypothetical data to examine the behaviour of each weighting method under certain assuptions.
 
