# Stigler's Diet Problem: GA
Nobel Laureate, George Stigler, identified the Diet Problem in 1939.  His goal was to find the cheapest set of ingredients to satisfy the minimum annual nutritional needs of an average adult male.  Stigler made a list of 77 food items and their respective nutritional contents. The average annual minimum nutritional intake for an adult male is:

Item	Amount	Unit
Calories	1095	Kilo Calories
Protein	25550	grams
Calcium	292	grams
Iron	4380	mg
Vitamin A	1825000	IU
Thiamine VB1	657	mg
Riboflavin VB2	985.5	mg
Niacin	6570	mg
Ascorbic Acid VC	27375	mg

At the time, this optimization problem was impossible to solve analytically and Stigler had to rely on educated guesswork to find his solution.  Stigler found that by selecting appropriate quantities of the food items (not all 77 items were included in his final solution) he could meet the annual dietary requirements for $39.93 per year (1939 prices).  

Dantzig’s simplex algorithm was applied to the Diet Problem in 1947.  Nine clerks performed calculations for more than two weeks to find the best solution, which came to $39.69 (Stigler was thus off by only 24 cents). 

You have to solve the Diet Problem using Computational Intelligence optimization algorithms.  The 77 food items, with their nutritional information per $1, can be found in DietProblem.xls (i.e. each line contains the mass and nutritional content that you can buy of the specific item with one dollar).  Sheet2 of the spreadsheet contains the required annual nutritional needs as given in the table above.  The chromosomes (individuals), all of length 77, will consist of real values each representing the weight (in grams) of each of the food items that should be included in the final annual diet. 

The real challenge in this assignment is finding an appropriate fitness function.  Be creative.  The fitness function should reward individuals for containing at least the required nutrition AND be for being inexpensive.

Three different optimization algorithms are to be investigated:

-	Adapt your Genetic Algorithm (GA) from Assignment 3
-	Also evaluate the optimization ability of the Differential Evolution (DE) algorithm, as well as that of the
-	Particle Swarm Optimization (PSO) algorithm

To be clear:  optimize the diet problem using each of the three algorithms listed above.  

Write a report that clearly contrasts the performance and effectiveness of the GA, DE and PSO algorithms.  Also discuss parameter values used in each algorithm with motivation for your choice of these values, e.g. mutation and crossover probability, scaling factor etc. 
