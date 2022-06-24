# Local-Volatility-Surface
Local Volatility interpolation

To compute the local volatility at each moneyness and maturity I had first to interpolate the IV surface ensuring no arbitrage is present. This means absence of negative calendar spreads and butterfly spread. To do so I have tried several approaches and ultimately went for a cubic spline interpolation. Once the volatiltiy surface had been correctly interpolated I have used the implied volatility formula proposed by Gatheral in terms of log-moneyness
