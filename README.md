# Credit-Card-Portfolio-Optimization-using-Python-Pulp-Package-

This project is two fold, The first part is simulating the credit card portfolio data using basic variables, The second part is Optimization using Pulp Package Liner Programming



<h2> 1)simulating the credit card data basic variables such as: </h2>

- account_id	,
- credit_limit( current),
- spend_percent	
- interest_rate_pct	,
- prob_of_default ( This can be considered as proxy for Fico score )
- revolving_spend ( derived by multiplying spend percernt , also known as utilization percent)
- fee_revenue,( assuming this to be 1 % and can be different , this included both late fee and merchant fee )
- interest_revenue, ( interest paid by consumer for the spend , anualized for the purpose of this project )
- total_revenue ( This is sum of interest revenue and the fee revenue , annualized for the purpose of this project)
- loss_given_default ( taken as multiple of probability of default and spend percent )
- Net_Profit_Before_Opti, 
- min_credit_limit : Assuming that we cannot reduce the credit limit for this case 
- max_credit_limit : Assuming this to be either 20 % more than that of current credit limit or at most 25000 which ever is lower)

 <h2> 2) The second part is Optimization :  </h2>

Here we define the objective function: Here we are trying to maximize the Net Profit 
and give constraints and then solve.
![image](https://user-images.githubusercontent.com/20480964/224130780-2229ec4e-a0ee-4f63-9b61-97a18a9a2db0.png)

Constraints :  <br /> 
Lower Limit of credit limit should be same as current limit  <br /> 
Upper Limit of credit limit should be either 20 % more than that of current credit limit or at most 25000 which ever is lower


 
