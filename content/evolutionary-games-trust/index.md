---
title: Evolutionary game theory and trust
summary: Evolutionary games focused on trust and socio-economical complex problems
date: "2021-05-28T00:00:00Z"

reading_time: false  # Show estimated reading time?
share: false  # Show social sharing links?
profile: false  # Show author profile?
comments: false  # Show comments?

# Optional header image (relative to `static/media/` folder).
header:
  caption: ""
  image: ""
---



Current Manuel's research track is called *Managing Complexity with Computational Intelligence (MACOI)*.

MACOI focuses on applying computational intelligence techniques for solving complex real-world applications and SME needs. The set of advanced computational techniques includes metaheuristics for single and multi-objective optimization problems, machine learning, simulation, agent-based modeling, and social network analysis. The target business and engineering applications are manifold: a) climate change, b) marketing, c) sharing economy, d) industrial engineering, e) healthcare, f) food engineering, or g) ecological modelling. We can highlight 5 main areas of the **MACOI** research line:



## Evolutionary game theory for trust dynamics 



{{% staticref "https://drive.google.com/open?id=0B5F5W-ZR7TDXOFdjUU1ZSnRHakU" "newtab" %}}Source code, runnable JAR and documentation{{% /staticref %}}



Trust and trustworthiness are of great importance in social and human systems, especially when considering managerial and economic decision-making. In this paper, we investigate the emergent dynamics of an evolutionary game-theoretic model - the N-player evolutionary trust game - consisting of three types of players: an investor, a trustee who is trustworthy, and a trustee who is untrustworthy. Here, we limit the interactions between players to local neighborhoods defined by a specific spatial topology or social network. Players are able to adjust their game-playing strategies using an evolutionary update rule based on the payoffs obtained by their neighbors. Through comprehensive simulation experiments, we find that it is possible to promote trust when players interact in a social network even if there is a substantial number of untrustworthy individuals in the initial population.


{{< figure library="true" src="network_trust_example_improved.png" lightbox="true" >}}



These results differ from findings reported for an unstructured population of the same game, where the existence of a single untrustworthy individual would eliminate trust completely. We compare the dynamics of the model with different social network densities and structures (e.g., from regular lattices to scale-free and random networks). We observe that the levels of trust vary under different network structures, and the level is correlated with how "difficult" the game is.

When game conditions are easy (i.e., low temptation to defect and/or almost no initial untrustworthy trustees), homogeneous networks with higher densities can promote higher levels of trust. However, when the game becomes harder, heterogeneous social networks with lower densities are able to promote higher levels of trust and global net wealth.

Keywords: Trust, Evolutionary Game Theory, Social Networks, Scale-free Networks, Agent-based Modeling.
 

{{% staticref "files/chica_et_al_ieee_tec_2017.pdf" "newtab" %}}Paper published in IEEE Transactions on Evolutionary Computation{{% /staticref %}}

 
## Our study on modelling trust for the sharing economy

In this paper, we present an evolutionary trust game to investigate the formation of trust in the so-called sharing economy from a population perspective. To the best of our knowledge, this is the first attempt to model trust in the sharing economy using the evolutionary game theory framework. Our sharing economy trust model consists of four types of players: a trustworthy provider, an untrustworthy provider, a trustworthy consumer, and an untrustworthy consumer. Through systematic simulation experiments, five different scenarios with varying proportions and types of providers and consumers were considered. Our results show that each type of players influences the existence and survival of other types of players, and untrustworthy players do not necessarily dominate the population even when the temptation to defect (i.e., to be untrustworthy) is high. Our findings may have important implications for understanding the emergence of trust in the context of sharing economy transactions.

{{< figure library="true" src="evolutionary_games_trust_sharing_economy.png" lightbox="true" >}}


**More info about this work:**


{{% staticref "files/paper_ieee-cec17-trust.pdf" "newtab" %}}IEEE CEC 2017 Paper{{% /staticref %}}

{{% staticref "files/mchica_trust_sharing_economy.pdf" "newtab" %}}Talk at the IEEE CEC 2017, in Donostia / San Sebastian{{% /staticref %}}

