# Analysis of a Supermarket 

This project analyzes sales and operational expenses for a supermarket, using a dataset loaded from a CSV file consisting on profits from transactions in another community with a similar socioeconomic level to the one to be reached which already include the payment of taxes, as well as the costs for the purchase of the products. The goal is to understand the supermarket's financial situation by fitting sales data to a beta distribution, calculating statistical measures and giving feedback to the owners of the supermarket. 

# Statistical Modelling 

The beta distribution is a family of continuous probability distributions defined on the interval [0, 1] in terms of two positive parameters, denoted by α and β.

$B(\alpha,\beta) =
\int_0^1 x^{\alpha-1}(1-x)^{\beta-1} dx$

I fitted a beta probability density function to represent the distribution of the data, due to its great flexibility to fit different distributions.
To determine the α and β parameters of the distribution, the *maximum likelihood estimation* method is used.

# Calculation of Operation Costs

The total expenses contemplated are as follows:

* 1.15x the minimum salary of:
    * 30 cashiers
    * 40 warehouse personnel
    * 40 people who serve customers in the aisles
    * 20 cleaning personnel
(Minimum salaries are taken from the General and Professional Minimum Wage Table provided from the National Minimum Wage Commission)
https://www.gob.mx/conasami/documentos/tabla-de-salarios-minimos-generales-y-profesionales-por-areas-geograficas

* One general manager with a salary of $100,000 per month 
* 4 assistant managers with a salary of $45,000 per month each.
  
* Electricity: 120 kW per hour per squared meter is taken into account in an area of 2000 squared meters, and with a cost of $2.3 kW per hour.
* Water:
    * Cost per cubic meter consumed: $169 179.28
    * Sanitation: $20,301.51
    * Sewerage: $16 917.93
    * VAT: $33,023.79
* Waste management: $2,708.82 for four days of collection per week.

# Insights

It would be necessary to convince 22.4% of the population to cover the estimated expenses and also have a profit of $1.5 million with a probability of 0.99. On the other hand, taking a sample of 5 people, the probability that the average of their ratings is greater than or equal to 8.5 is 0.0234. These probabilities are very low, so it is necessary to take measures to improve the perception of the supermarket among customers, and thus make more people prefer this supermarket over others.

# Run the analysis 
You must have downloaded the CSV file included in the repository (SuperMarketData.csv) and include it in the environment where you want to run the program.

