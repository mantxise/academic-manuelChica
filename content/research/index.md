---
title: MACOI Research Line
summary: Main insights about Manuel's research line
date: "2018-06-28T00:00:00Z"

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


* **MACOI#1** _Use of evolutionary game theory (EGT) and agent-based modeling (ABM) for social dilemmas and economical/social problems._ We have applied the models to climate change problems or to trust issues in societies (see an example below). Also, we have used ABM for modeling migrations.

* **MACOI#2** _Artificial intelligence and social simulation in Marketing._ Different approaches and methods are applied to marketing, from ABM to system dynamics and optimization methods.

* **MACOI#3** _Metaheuristics for industrial and economical problems._ In this line we use metaheuristics (e.g., evolutionary computation and evolutionary multiobjective optimization methods) to optimize industrial systems such as assembly lines. Apart from the optimization method itself, we also apply methods to incorporate specific knowledge from the experts and to guide the optimization process to find the most suitable solution.

* **MACOI#4** _Metaheuristics for model validation_ It is easy to generate a model but it is difficult to have a rigorous and valid model. The objective of this line is to provide modelers and stakeholders with automatic tools to increase their confidence in the model.

* **MACOI#5** _Explanaible artificial intelligence and advanced modeling._ The goal of this line is to generate more explanaible AI model such as using linguistic information with fuzzy logic, or causal diagrams to help experts when making decisions.



{{< figure library="true" src="complex_systems.png" lightbox="true" >}}


{{% staticref "files/ulpgc_seminar_mchica.pdf" "newtab" %}}Talk about ABM and complex systems at ULPGC{{% /staticref %}}


We list below a couple of examples of this research line.


{{% toc %}}



## Modeling and building agent-based DSS for marketing


This research project is related to our [JMR publication]({{< ref "/publication/chica-17-jmr/index.md" >}}), co-authored by Dr. Manuel Chica and Dr. William Rand, from the Poole College of Management, North Carolina State University.  Different media covered our work, such as Daily Science. See our [post]({{< ref "/post/media_JMR_2017/index.md" >}})

**Abstract**

Marketers have to constantly make decisions on how to implement word-of-mouth (WOM) programs and a well-developed decision support system (DSS) can provide them with valuable assistance. The authors propose an agent-based framework that aggregates social network-level individual interactions to guide the construction of a successful DSS for WOM.

The framework presents a set of guidelines and recommendations to:
1. involve stakeholders,
2. follow a data-driven iterative modeling approach,
3. increase validity through automated calibration and,
4. understand the DSS behavior.

This framework is applied to build a DSS for a freemium app, where premium users discuss the product with their social network and promote the viral adoption. After its validation, the agent-based DSS forecasts the aggregate number of premium sales over time and the most likely users to become premium in a near future. The experiments show how the DSS can help managers by forecasting premium conversions and increasing the number of premiums via targeting and reward policies.

**Keywords:** Word-of-mouth, Marketing Decision Support Systems, Agent-based Modeling, Targeting and Referrals, Freemium Business Model


**Research questions**

We were approached by the firm to help answer the question how can they incentivize additional conversions? We quickly determined that word-of-mouth seemed to have a large impact on conversions, but the firm did not know how to use that knowledge, so we hypothesized that it would be possible to create an agent-based model that used social network data to assist them in targeting users who would have a large impact on overall conversions.

**Our method**

We first constructed an agent-based model that attempted to predict the rate of conversions in a massive-online game, called Animal Jam. The main components of this model were a social network and a model of social influence propagation. Once we had a model that we had shown was accurate at predicting out-of-sample conversions, we then constructed a tool that enabled the examination of the effects of different marketing policies on the social network. Using this model we were able to explore the role of targeting different users with different incentives:


{{< figure library="true" src="freemium-not-really.jpg" lightbox="true" >}}


**Findings**

We created a set of guidelines that can be generally used to construct a decision support system for understanding word-of-mouth marketing in a wide variety of domains. In the Animal Jam case, we determined that targeting users who already had a large number of premium friends but who had not converted themselves was likely to have the largest effect on conversion rates, both in terms of the targeted users, but also in terms of spillovers to network peers.


{{< figure library="true" src="steps_framework_revised_final.png" lightbox="true" >}}


**Implications**

These findings illustrate how we can build analytic tools to help create more data driven decisions in a wide variety of contexts. Managers should shift away from the more intuition -based design of campaigns and instead refocus on data-driven, simulation-supported decision support tools. In particular, our application has implications for most freemium apps that are interested in encouraging a larger conversion rate.

{{< figure library="true" src="dss_run_scenarios.png" lightbox="true" >}}


The figure below illustrates the effect of incentivizing 2,000 non-premium users in terms of the number of additional conversions that will happen within the following month. As can be seen, the largest increase happens if the most likely users (>= 6 premium friends already) are targeted:


{{< figure library="true" src="add_premiums.png" lightbox="true" >}}


**Souce code, data-sets, and documentation**

{{% staticref "https://bitbucket.org/mchserrano/socialdynamicsfreemiumapps" "newtab" %}}Bitbucket Git Repository{{% /staticref %}}


{{% staticref "https://www.openabm.org/model/5191" "newtab" %}}OpenABMs.org node{{% /staticref %}}

 
**Realted talks**

{{% staticref "files/mchica_netscix_wroclaw.pdf" "newtab" %}}Talk at the NetSciX conference, Wroclaw{{% /staticref %}}

{{% staticref "files/talk_mchica_areces.pdf" "newtab" %}}Keynote talk at the Marketing Series by Catedra Ramon Areces, Oviedo 2015 (in Spanish){{% /staticref %}}




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

