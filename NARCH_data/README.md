<div style="margin: 0; padding: 0; text-align: center; border: none;">
<a href="https://quantlet.com" target="_blank" style="text-decoration: none; border: none;">
<img src="https://github.com/StefanGam/test-repo/blob/main/quantlet_design.png?raw=true" alt="Header Image" width="100%" style="margin: 0; padding: 0; display: block; border: none;" />
</a>
</div>

```
Name of Quantlet: NARCH_data

Published in: Spatial Effects and Uncertainty in Cryptocurrencies: the case of Network ARCH Models

Description: Builds the balanced panel of 50 cryptocurrencies over 1517 consecutive trading days, from 6 January 2021 to 2 March 2025, that underlies the network ARCH study, and produces the two descriptive figures motivating it. Starting from the top 100 coins by market capitalisation, a coin is retained only if it is fully observed on price, volume and market capitalisation over a common window, and the window is chosen to maximise the number of fully observed coin-day observations. Six coins are excluded: three for insufficient history, two for discontinuous listings and one for long runs of zeros that become non-finite under the log transform. Gaps are never imputed, since interpolation would insert smooth artificial structure into the co-movement of volatility that the study sets out to measure. The script reports that the pipeline finiteness guard never fires on the retained panel, so no value in it has been replaced. Prices and volumes are converted to daily logarithmic changes, which are additive over time and symmetric in gains and losses. The average pairwise return correlation is 0.46 for prices and 0.34 for volumes.

Keywords: balanced panel, data cleaning, missing data, window selection, log returns, volatility clustering, cryptocurrency, replicability, descriptive statistics

Author: Mihai-Adrian Achim, Stefana Belbe, Codruta Mare, Philipp Otto

See also: NARCH_weights, NARCH_meanfilter, NARCH_estimation, NARCH_diagnostics, https://github.com/MUSET-TE/spatial_crypto

Submitted: 11. Nov 2026, Mihai-Adrian Achim

Datafile: market_cap_top_100.csv, prices_top_100.csv, volumes_top_100.csv

Output: NARCH_data.png, returns_prices.csv, returns_volumes.csv

```
<div align="center">
<img src="https://raw.githubusercontent.com/QuantLet/spatial_crypto/main/NARCH_data/NARCH_data.png" alt="Image" />
</div>

