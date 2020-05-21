---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "PhD Thesis"
summary: "My PhD thesis is about the application of multiobjective biologically-inspired metaheuristics: Ant Colony Optimization (ACO) and Genetic Algorithms to solve the Time and Space Assembly Line Balancing Problem (TSALBP)."
authors: []
tags: []
categories: []
date: 2020-05-21T14:07:18+02:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: "https://manuchise.wordpress.com/more-about-phd-manuel-chica/"
url_pdf: "http://hdl.handle.net/10481/20200"
url_slides: "https://manuchise.files.wordpress.com/2019/02/presentacion_tesis_mchica.pdf"
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---


## What are metaheuristics, genetic algorithms and ant colony optimization?

Many complex combinatorial and numerical optimization problems arise in human activities, such as economics (e.g., portfolio selection), industry (e.g., scheduling or logistics), or engineering (e.g., network routing), among many others.

{{< figure library="true" src="manuel_chica_phd1.png" lightbox="true" >}}

Using classical algorithmic techniques to get optimal solutions for this kind of problems in reasonable time is difficult. This fact has favored the development of different approximate algorithm methodologies in the last two decades such as metaheuristics. Metaheuristics are able to quickly provide high quality solutions and particularly useful to solve these problems due to their flexibility, their iterative nature, and their capability to simultaneously optimize several conflicting criteria. 

They constitute a diverse family of optimization algorithms including methods such as simulated annealing, tabu search, multi-start methods, iterated local search, variable neighborhood search, GRASP etc. The most successful are biologically inspired like the Genetic Algorithms, Memetic Algorithms, PSO, and Ant Colony Optimization (ACO).


## The industrial problem: TSALBP

An assembly line is a flow-oriented production system made up of a number of workstations, arranged in series and in parallel. Assembly lines are of great importance in the industrial production of high quantity standardized commodities and more recently even gained importance in low volume production of customized products. The assembly line configuration involves determining an optimal assignment of a subset of tasks to each station of the plant to minimize the inefficiency of the line or its total downtime while respecting all the constraints imposed on the tasks and on the stations such as the . Such problem is called assembly line balancing (ALB) and it is a very complex combinatorial optimization problem (known to be NP-hard) which has become an active field of research over more than half a century.

{{< figure library="true" src="graph_tsalbp.png" title="A precedence graph which represents the first 8 tasks of the real-world instance of Nissan. Time and area information are shown next to each task. Task 31 is also shown because of its precedence relation with respect to task 2." lightbox="true" >}}


A more realistic extension of assembly line balancing is one proposed by Bautista (www.nissanchair.com/TSALBP), which considers an additional space constraint to get a simplified but closer version to real-world problems, defining the Time and Space ALB problem (TSALBP). TSALBP presents eight variants depending on three optimization criteria: the line cycle time $c$, the number of stations $m$, and their area $A$. Four of those variants present a multi-objective nature.

$$ f^1(x) =  m =  \sum_{k=1}^{UB_{m}} \max_{j \in J} \{ x_{jk}  \}$$

$$ f^2(x) =  c =  {  \max_{k \in K} \{ \sum_{j=1}^{|J|} \overline{t}_{j\varepsilon^0}x_{jk} \} }$$

$$ f^3(x) =  A =  {  \max_{k \in K} \{ \sum_{j=1}^{|J|} \overline{a}_{j\varepsilon^0}x_{jk} \} }$$


## Metaheuristics and multiobjective optimization

*Ant Colony Optimization (ACO)* is a population-based metaheuristic that can be used to find approximate solutions to difficult optimization problems. In ACO, a set of software agents called artificial ants search for good solutions to a given optimization problem. To apply ACO, the optimization problem is transformed into the problem of finding the best path on a weighted graph. The artificial ants incrementally build solutions by moving on the graph. The solution construction process is stochastic and is biased by a pheromone model, that is, a set of parameters associated with graph components (either nodes or edges) whose values are modified at runtime by the ants.

*Genetic algorithms (GAs)* were formally introduced in the 1970s by John Holland at University of Michigan. The continuing price/performance improvements of computational systems has made them attractive for some types of optimization. In particular, genetic algorithms work very well on mixed (continuous and discrete) combinatorial problems. They are less susceptible to getting "stuck" at local optima than gradient search methods. To use a genetic algorithm you must represent a solution to your problem as a genome (or chromosome). The genetic algorithm then creates a population of solutions and applies genetic operators such as mutation and crossover to evolve the solutions in order to find the best one(s).




