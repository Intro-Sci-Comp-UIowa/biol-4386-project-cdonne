# IsotopeR parameters 
The default parameters are as follows
```
- Number of [Markov] chains: 3
- MCMC burn-in: 1000
- MCMC runs: 1000
- Thinning rate: 1
- Plot observations: TRUE 
- Plot mixing estimates: TRUE
- Plot dietary source contributions: TRUE 
- Run parallel: TRUE 
```

The only parameter changed for reproducing Figure 5 was 

` Plot dietary source contributions: False `

Turning this parameter off means the program will not produce a dietary source contributions graph. This graph is not necessary for this project. 