<div style="margin: 0; padding: 0; text-align: center; border: none;">
<a href="https://quantlet.com" target="_blank" style="text-decoration: none; border: none;">
<img src="https://github.com/StefanGam/test-repo/blob/main/quantlet_design.png?raw=true" alt="Header Image" width="100%" style="margin: 0; padding: 0; display: block; border: none;" />
</a>
</div>

```
Name of Quantlet: NARCH_meanfilter

Published in: Spatial Effects and Uncertainty in Cryptocurrencies: the case of Network ARCH Models

Description: Stage 1 of the two-stage network ARCH pipeline: a spatiotemporal ARMA mean filter estimated coin by coin by maximum likelihood, carrying the contemporaneous and the lagged row-standardised neighbour return as external regressors. The stage exists to break a circularity. The neighbourhood matrix is built from return correlations, so estimating volatility dependence directly on raw returns would recover the structure that was inserted by hand, and the spatial parameter would measure return co-movement rather than volatility transmission. Filtering the conditional mean first leaves innovations explained neither by a coin own past nor by what its neighbours did today or yesterday, and only their magnitude is passed to stage 2. The contemporaneous neighbour regressor is admissible here because cryptocurrency markets trade continuously, with no closing auction behind which a lagged effect could hide. The filter removes a median of 55 percent of return variance for prices and 43 percent for volumes, while leaving the dependence in the squared innovations intact, which is exactly what stage 2 is meant to model.

Keywords: ARMA, mean filter, spatiotemporal, external regressors, innovations, endogeneity, circularity, cryptocurrency, volatility network, spatial ARCH

Author: Mihai-Adrian Achim, Stefana Belbe, Codruta Mare, Philipp Otto

See also: NARCH_data, NARCH_weights, NARCH_estimation, NARCH_diagnostics, https://github.com/MUSET-TE/spatial_crypto

Submitted: 11. Nov 2026, Mihai-Adrian Achim

Datafile: returns_prices.csv, returns_volumes.csv

Output: NARCH_meanfilter.png, innovations_prices.csv, innovations_volumes.csv

```
<div align="center">
<img src="https://raw.githubusercontent.com/QuantLet/spatial_crypto/main/NARCH_meanfilter/NARCH_meanfilter.png" alt="Image" />
</div>

