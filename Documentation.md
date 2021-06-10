Documentation
================

-   [1 Ternary Networks](#ternary-networks)
    -   [1.1 Example](#example)
-   [2 *SteadyCellPhenotype* tools](#tools)

# 1 Ternary Networks

A ternary network is a pair 𝒯 = (*G*,*F*), where *G* is a digraph on *n*
nodes and
*F* = (*f*<sub>1</sub>,…,*f*<sub>*n*</sub>) : {0, 1, 2}<sup>*n*</sup> → {0, 1, 2}<sup>*n*</sup>
is a global transition function. Each node *v* in *G* takes on the
values in the set {0, 1, 2} and is updated by a local activation
function *f*<sub>*v*</sub> : {0, 1, 2}<sup>*n*</sup> → {0, 1, 2}. The
value of the function *f*<sub>*v*</sub> depends on its input nodes and
their current state. The update schedule is *synchronous* meaning that
all nodes in the network are updated simultaneously.

## 1.1 Example

To make terminology precise and clear we will use one of our previously
published models of intracellular iron metabolism
<https://doi.org/10.1371/journal.pcbi.1005352>. We have selected a
portion of the network termed *Iron Homeostasis Pathway* in the article
(Fig 1. Intracellular iron network). Note that Hepcidin was excluded,
which resulted in the network on six nodes (image below). We will also
demonstrate functionalities and tools of the *SteadyCellPhenotype* on
the full 24-node model (see Section [*SteadyCellPhenotype*
tools](#tools)).

![Iron Model 2017.](Iron_core.png)

# 2 *SteadyCellPhenotype* tools
