# statistical-distances
A python module with distance measures between two probability density functions. The measures can be applied to compare points in vector spaces (vectors of the same size).

## Requirements
* [Python](https://www.python.org) >= 3.6
* [numpy](http://www.numpy.org) >= 1.16.4
 > Use pip to install: `python3 -m pip install numpy`

## Usage

```python
import numpy as np
from distance import Distance

d = Distance()
v1 = np.array([0.2, 0.4, 0.2, 0.2])
v2 = np.array([0.7, 0.1, 0.1, 0.1])

print(d.euclidean(v1, v2))
# 0.6

print(d.google(v1, v2))
# 0.5
```

## Distance measures

| Distance | Synonymes | References |
| ----------- | ----------- | --------- |
| ACC distance | Average distance | [8, 15] |
| Addictive Symmetric Chi-square distance | - | [15] |
| Bhattacharyya distance | - | [1, 15] |
| Bray-Curtis distance | Sørensen distance, Bray-Curtis dissimilarity | [2, 15] |
| Canberra distance | - | [15] |
| Chebyshev distance | Chessboard distance, King-move metric, Maximum value distance, Minimax approximation | [15] |
| Clark distance | - | [15] |
| Cosine distance | - | [17] |
| Czekanowski distance | - | [15] |
| Dice dissimilarity | - | [4, 15] |
| Divergence | - | [15] |
| Euclidean distance | Pythagorean metric | [15] |
| Gower distance | - | [6, 15] |
| Hellinger distance | - | [15] |
| Intersection distance | Non-overlaps | [15] |
| Jaccard distance | - | [15] |
| Jeffreys divergence | J divergence | [7, 15] |
| Jensen-Shannon divergence | - | [12, 15] |
| K divergence | - | [15] |
| Kulczynski distance | - | [15] |
| Kullback-Leibler divergence | KL divergence, relative entropy, information deviation |
| Kumar-Johnson distance | - | [10, 15] |
| Lorentzian distance | - | [15] |
| Manhattan distance | City block distance, Rectilinear distance, Taxicab norm | [15] |
| Maryland Bridge distance | - | [3] |
| Matusita distance | - | [15] |
| Minkowski distance | - | [15] |
| Motyka distance | - | [15] |
| Neyman chi-square distance | - | [13, 15] |
| Normalized Google Distance (NGD) | - | [11] |
| Pearson chi-square divergence | - | [14, 15] |
| Penrose shape distance | - | [3] |
| Soergel distance | - | [15] |
| Squared chi-square distance | Triangular discrimination | [15] |
| Squared Euclidean distance | - | [5, 15] |
| Squared-chord distance | - | [5, 15] |
| Taneja distance | - | [15, 16] |
| Tanimoto distance | - | [15] |
| Topsøe distance | Information statistic | [15] |
| Vicis Symmetric chi-square distance | - | [15] |
| Vicis-Wave Hedges distance | - | [15] |
| Wave Hedges distance | - | [15] |


## References

1. Bhattacharyya A (1947) On a measure of divergence between two statistical populations defined by probability distributions, Bull. Calcutta Math. Soc., 35, 99–109.

2. Bray JR, Curtis JT (1957) An ordination of the upland forest of the southern Winsconsin. Ecological Monographies, 27, 325-349.

3. Deza M, Deza E (2009) Encyclopedia of Distances. Springer-Verlag Berlin Heidelberg. 1-590.

4. Dice LR (1945) Measures of the amount of ecologic association between species. Ecology. 26, 297-302.

5. Gavin DG et al. (2003) A statistical approach to evaluating distance metrics and analog assignments for pollen records. Quaternary Research 60:356–367.

6. Gower JC. (1971) General Coefficient of Similarity and Some of Its Properties, Biometrics 27, 857-874.

7. Jeffreys H (1946) An Invariant Form for the Prior Probability in Estimation Problems. Proc.Roy.Soc.Lon., Ser. A 186, 453-461.

8. Krause EF (2012) Taxicab Geometry An Adventure in Non-Euclidean Geometry. Dover Publications. ISBN-13: 978-0486252025.

9. Kullback S, Leibler RA (1951) On information and sufficiency. Ann. Math. Statist. 22:79–86

10. Kumar P, Johnson A. (2005) On a symmetric divergence measure and information inequalities, Journal of Inequalities in pure and applied Mathematics. 6(3).

11. Lee & Rashid (2008) Information Technology, ITSim 2008. doi:10.1109/ITSIM.2008.4631601.

12. Lin J. (1991) Divergence measures based on the Shannon entropy. IEEE Transactions on Information Theory, 37(1):145–151.

13. Neyman J (1949) Contributions to the theory of the chi^2 test. In Proceedings of the First Berkley Symposium on Mathematical Statistics and Probability.

14. Pearson K. (1900) On the Criterion that a given system of deviations from the probable in the case of correlated system of variables is such that it can be reasonable supposed to have arisen from random sampling, Phil. Mag. 50, 157-172.

15. Sung-Hyuk C (2007) Comprehensive Survey on Distance/Similarity Measures between Probability Density Functions. International Journal of Mathematical Models and Methods in Applied Sciences. vol. 1(4), pp. 300-307 [[pdf](http://www.fisica.edu.uy/~cris/teaching/Cha_pdf_distances_2007.pdf)].

16. Taneja IJ. (1995) New Developments in Generalized Information Measures, Chapter in: Advances in Imaging and Electron Physics, Ed. P.W. Hawkes, 91, 37-135.

17. Virtanen P. (2020) SciPy 1.0: fundamental algorithms for scientific computing in Python. Nature Methods. 17, 261–272. [[10.1038/s41592-019-0686-2](https://doi.org/10.1038/s41592-019-0686-2)].