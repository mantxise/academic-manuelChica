---
title: MACOI Research Line
summary: Main insights about Manuel's research line
date: "2018-06-28T00:00:00Z"

reading_time: false  # Show estimated reading time?
share: false  # Show social sharing links?
profile: false  # Show author profile?
comments: false  # Show comments?

# Optional header image (relative to `static/img/` folder).
header:
  caption: ""
  image: ""
---



Current Manuel's research track is called *Managing Complexity with Computational Intelligence (MACOI)*.

MACOI focuses on applying computational intelligence techniques for solving complex real-world applications and SME needs. The set of advanced computational techniques includes metaheuristics for single and multi-objective optimization problems, machine learning, simulation, agent-based modeling, and social network analysis. 

The target business and engineering applications are manifold: 

* climate change,
* marketing, 
* sharing economy,
* industrial engineering, 
* healthcare, 
* food engineering,
* ecological modelling.

{{< figure library="true" src="complex_systems.png" lightbox="true" >}}


We list below some research examples.


## Modeling and building agent-based DSS for marketing


This research project is related to our [JMR publication]({{< ref "/publication/chica-17-jmr/index.md" >}}), co-authored by Dr. Manuel Chica and Dr. William Rand, from the Poole College of Management, North Carolina State University.  Different media covered our work, such as Daily Science. See our [post]({{< ref "/post/media_JMR_2017/index.md" >}})

### Abstract

Marketers have to constantly make decisions on how to implement word-of-mouth (WOM) programs and a well-developed decision support system (DSS) can provide them with valuable assistance. The authors propose an agent-based framework that aggregates social network-level individual interactions to guide the construction of a successful DSS for WOM.

The framework presents a set of guidelines and recommendations to:
1. involve stakeholders,
2. follow a data-driven iterative modeling approach,
3. increase validity through automated calibration and,
4. understand the DSS behavior.

This framework is applied to build a DSS for a freemium app, where premium users discuss the product with their social network and promote the viral adoption. After its validation, the agent-based DSS forecasts the aggregate number of premium sales over time and the most likely users to become premium in a near future. The experiments show how the DSS can help managers by forecasting premium conversions and increasing the number of premiums via targeting and reward policies.

### Keywords
Word-of-mouth, Marketing Decision Support Systems, Agent-based Modeling, Targeting and Referrals, Freemium Business Model


### Research questions

We were approached by the firm to help answer the question how can they incentivize additional conversions? We quickly determined that word-of-mouth seemed to have a large impact on conversions, but the firm did not know how to use that knowledge, so we hypothesized that it would be possible to create an agent-based model that used social network data to assist them in targeting users who would have a large impact on overall conversions.

### Our method

We first constructed an agent-based model that attempted to predict the rate of conversions in a massive-online game, called Animal Jam. The main components of this model were a social network and a model of social influence propagation. Once we had a model that we had shown was accurate at predicting out-of-sample conversions, we then constructed a tool that enabled the examination of the effects of different marketing policies on the social network. Using this model we were able to explore the role of targeting different users with different incentives:


{{< figure library="true" src="freemium-not-really.jpg" lightbox="true" >}}


### Findings

We created a set of guidelines that can be generally used to construct a decision support system for understanding word-of-mouth marketing in a wide variety of domains. In the Animal Jam case, we determined that targeting users who already had a large number of premium friends but who had not converted themselves was likely to have the largest effect on conversion rates, both in terms of the targeted users, but also in terms of spillovers to network peers.


{{< figure library="true" src="steps_framework_revised_final.png" lightbox="true" >}}


### Implications

These findings illustrate how we can build analytic tools to help create more data driven decisions in a wide variety of contexts. Managers should shift away from the more intuition -based design of campaigns and instead refocus on data-driven, simulation-supported decision support tools. In particular, our application has implications for most freemium apps that are interested in encouraging a larger conversion rate.

{{< figure library="true" src="dss_run_scenarios.png" lightbox="true" >}}


The figure below illustrates the effect of incentivizing 2,000 non-premium users in terms of the number of additional conversions that will happen within the following month. As can be seen, the largest increase happens if the most likely users (>= 6 premium friends already) are targeted:


{{< figure library="true" src="add_premiums.png" lightbox="true" >}}


### Souce code, data-sets, and documentation


[Bitbucket Git Repository] (https://bitbucket.org/mchserrano/socialdynamicsfreemiumapps)
[OpenABMs.org node] (https://www.openabm.org/model/5191)

 
### Realted talks


{{% staticref "files/mchica_netscix_wroclaw.pdf" "newtab" %}}Talk at the NetSciX conference, Wroclaw{{% /staticref %}}
{{% staticref "files/talk_mchica_areces.pdf" "newtab" %}}Keynote talk at the Marketing Series by Catedra Ramon Areces, Oviedo 2015 (in Spanish){{% /staticref %}}

