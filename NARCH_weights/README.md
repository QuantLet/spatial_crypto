<div style="margin: 0; padding: 0; text-align: center; border: none;">
<a href="https://quantlet.com" target="_blank" style="text-decoration: none; border: none;">
<img src="https://github.com/StefanGam/test-repo/blob/main/quantlet_design.png?raw=true" alt="Header Image" width="100%" style="margin: 0; padding: 0; display: block; border: none;" />
</a>
</div>

```
Name of Quantlet: NARCH_weights

Published in: Spatial Effects and Uncertainty in Cryptocurrencies: the case of Network ARCH Models

Description: Builds and visualises the two spatial weight matrices used to define cryptocurrency neighbourhoods in the network ARCH model. Neighbours are derived from the correlation matrix of daily log returns, since coins have no geographical location. Two definitions are compared: an absolute correlation threshold at 0.15, selected for the price model, and a k-nearest-neighbour rule with k = 5, selected for the volume model. Both matrices are row-standardised, so each row sums to one and a weight is the share of a coin neighbourhood accounted for by one neighbour. Colour is scaled by quantile within each panel, because row standardisation ties the size of a weight to the number of neighbours, a median of 45 links for prices against exactly five for volumes.

Keywords: spatial weight matrix, adjacency matrix, row standardisation, correlation network, k-nearest-neighbour, cryptocurrency, volatility network, spatial ARCH, heatmap

Author: Mihai-Adrian Achim, Stefana Belbe, Codruta Mare, Philipp Otto

See also: NARCH_estimation, NARCH_data, https://github.com/MUSET-TE/spatial_crypto

Submitted: 21. Aug 2026, Mihai-Adrian Achim

Datafile: returns_prices.csv, returns_volumes.csv

Output: NARCH_weights.png

```
<div align="center">
<img src="https://raw.githubusercontent.com/QuantLet/spatial_crypto/main/NARCH_weights/NARCH_weights.png" alt="Image" />
</div>

