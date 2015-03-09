# HW3_brianhigh

Example HW3 for Biostat-578, Winter 2015.

## Requirements

- Assignment: [Homework #3: Differential gene expression and limma](https://github.com/raphg/Biostat-578/blob/master/HW3.md)

Quote:

<blockquote>
<p>
Reproduce the results presented in Figure 2 of the following paper: Qian, F., Bolen, C. R., Jing, C., Wang, X., Zheng, W., Zhao, H., et al. (2013). [Impaired toll-like receptor 3-mediated immune responses from macrophages of patients chronically infected with hepatitis C virus](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3571267/). Clinical and Vaccine Immunology : CVI, 20(2), 146–155. doi:10.1128/CVI.00530-12
</p>
<p>
You will have to:
<ol>
<li>Get the data from GEO
<li>Normalize the data (if necessary)
<li>Use limma to test for differential expression
<li>Display the results using a heatmap [Hint: Use the pheatmap package]
</ol>
</p>
</blockquote>

## Assignment Modification

As this is an example homework assignment, we will modify the assignment slightly. For this example, we will look through this 2005 case study -- [Estrogen Data
A 2x2 factorial experiment](http://www.bioconductor.org/help/course-materials/2005/BioC2005/labs/lab01/estrogen/) -- and use it as a guide to completing HW3 using a contrast matrix. The case study uses a very similar model, so the method should be directly applicable to the HW3 problem. In HW3, you have poly(I·C) (treatment vs. mock) and HCV infection (VL+ vs. VL-), whereas in the case study, they have two time periods after treatment and presence or absence of estrogen. So, the goal is to see if this approach (in particular, the creation and use of the contrast matrix) can be successfully applied to the analysis required to produce the fig. 2 heatmap of the HCV paper as described in HW3. Do the numbers of probes found using this method match the numbers reported in the paper? Does the heatmap match fig. 2 of the paper?
