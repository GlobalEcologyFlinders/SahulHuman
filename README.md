# SahulHuman
R code for reproducing age-structured models of ancient humans entering Sahul.

The repositories code and associated data are to reproduce the models presented in the following companion papers:

- BRADSHAW, CJA, S ULM, AN WILLIAMS, MI BIRD, RG ROBERTS, Z JACOBS, F LAVIANO, LS WEYRICH, T FRIEDRICH, K NORMAN, F SALTRÉ. In review. Minimum founding populations of the first people to colonise Australia. Nature Ecology and Evolution

- BIRD, MI, SA CONDIE, S O’CONNOR, D O’GRADY, C REEPMEYER, S ULM, M ZEGA, F SALTRÉ, CJA BRADSHAW. Accepted. Early human settlement of Sahul was not an accident. Scientific Reports

The first code ('humanpopmodelgithub.R) is a stochastic projection of the human population entering Sahul required to estimate minimum viable population size. It requires the following R libraries:

- boot
- tcltk
- sp
- rgdal
- raster

The code also requires the source code: 'matrixOperators.r' (provided in this repository), as well as the following data files:

- 'world2013lifetable.csv' (modern human demographic data from Bradshaw & Brook. 2014. Human population reduction is not a quick fix for environmental problems. Proceedings of the National Academy of Sciences of the USA 111: 16610–16615. doi:10.1073/pnas.1410465111)
- 'ClimateSahul_Npp.csv' (hindcasted net primary production values for northern Sahul produced by the LOVECLIM global circulation model)


The repository also includes a global sensitivity analysis ('ancienthumanfound_gsa_sim_func_v2.R) that uses the following R libraries:

- iterators
- snow
- doSNOW
- foreach
- lhs
- data.table

The sensitivity analysis also requires the source code: 'matrixOperators.r' (provided in this repository), as well as the following data files:

- 'ClimateSahul_Npp.csv' (hindcasted net primary production values for northern Sahul produced by the LOVECLIM global circulation model)
- 'world2013lifetable.csv' (modern human demographic data from Bradshaw & Brook. 2014. Human population reduction is not a quick fix for environmental problems. Proceedings of the National Academy of Sciences of the USA 111: 16610–16615. doi:10.1073/pnas.1410465111)

