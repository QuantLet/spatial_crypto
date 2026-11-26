<div style="margin: 0; padding: 0; text-align: center; border: none;">
<a href="https://quantlet.com" target="_blank" style="text-decoration: none; border: none;">
<img src="https://github.com/StefanGam/test-repo/blob/main/quantlet_design.png?raw=true" alt="Header Image" width="100%" style="margin: 0; padding: 0; display: block; border: none;" />
</a>
</div>

```
Name of Quantlet: NARCH_estimation

Published in: Spatial Effects and Uncertainty in Cryptocurrencies: the case of Network ARCH Models

Description: Stage 2 of the pipeline: the dynamic network ARCH model estimated by quasi-maximum likelihood under each of the three neighbourhood definitions, reproducing the full selection table of the paper. The model carries three parameters: rho for contemporaneous spatial dependence, gamma for temporal persistence and delta for the spatiotemporal transmission of neighbours past volatility. Two estimation points are handled explicitly. The contemporaneous spatial lag is endogenous by construction, since coin j log-volatility today is a regressor in coin i equation while coin i is a regressor in coin j, so least squares is inconsistent rather than merely inefficient. Identification comes from the log-determinant term of the quasi-likelihood: without it the criterion reduces to a sum of squares that the optimiser can shrink by driving rho towards one, so spillover would be reported for any series at all. All six cells of the grid are reported rather than only the two selected, because that is the evidence that the price versus volume contrast does not depend on how the neighbourhood was defined: rho stays in 0.346 to 0.500 for prices and in 0.116 to 0.280 for volumes, and the two ranges never meet. A coin left with an all-zero row of W, which happens to dexe under the threshold rule on volumes, is filtered without the neighbour terms, since those drop out of its mean equation by construction.

Keywords: spatial ARCH, quasi-maximum likelihood, Jacobian, log-determinant, endogeneity, simultaneity, model selection, information criteria, cryptocurrency, volatility spillover

Author: Mihai-Adrian Achim, Stefana Belbe, Codruta Mare, Philipp Otto

See also: NARCH_data, NARCH_weights, NARCH_meanfilter, NARCH_diagnostics, https://github.com/MUSET-TE/spatial_crypto

Submitted: 11. Nov 2026, Mihai-Adrian Achim

Datafile: returns_prices.csv, returns_volumes.csv

Output: NARCH_estimation.png, estimates.csv

```
<div align="center">
<img src="https://raw.githubusercontent.com/QuantLet/spatial_crypto/main/NARCH_estimation/NARCH_estimation.png" alt="Image" />
</div>

