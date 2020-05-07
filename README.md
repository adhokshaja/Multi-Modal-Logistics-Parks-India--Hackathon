# Multi-Modal-Logistics-Parks-India--Hackathon
A transport network optimization problem attempted as a part of the IGSA UW-Madison SUPPLY CHAIN HACKATHON - April 2020

## Problem Statement
Development of Multi-Modal Logistics Parks (MMLP) at strategic locations to enable efficient inter-modal (road,
rail, waterway and air) freight movement and formalised interface amongst logistics service providers, service
users and regulators is expected to bring about significant efficiencies in India’s logistics sector, providing a
much-needed impetus towards driving logistics cost to less than 10% of country’s GDP. To achieve that goal, the
government has embarked on ambitious journey to develop a network of MMLPs across the country. The
complexities involved in its implementation, criticality of the infrastructure and need for smooth operations
involving multiple stakeholders necessitates strong focus from the government on its development and
operations. This becomes more important especially in the current unprecedented challenging times of COVID-
19.
In this question, we would solve a Minimum-cost flow problem, which is an optimization problem to find the
cheapest possible way of sending a certain amount of flow through a flow network. The flow network is the
above described network of ports to possible MMLP locations with the nodes being either source or demand
nodes and the edges being the distance between nodes. The Data File is a dense matrix where the rows index
are the ports and the column index are the demand zones to be satisfied. The matrix itself is the distance
between these locations in kilometer (km). The cost per kilometer is 35 Rs. Find the minimum cost to satisfy the
demand.


## Author's notes
This has been adapted to python from the Julia Jupyter Notebook files provided.
The names for cities/ports in the original distance csv were not consistant with the city/port in the supply
demand excel file. These have been corrected to be made consistent before import
In addition to pandas this solution uses pyomo with glpk solver. These can be installed in a Conda
environment by using
```
conda install -c conda-forge glpk
conda install -c conda-forge pyomo
```
