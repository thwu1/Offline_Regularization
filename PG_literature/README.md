### Iteration complexity for Tabular + softmax parameterization with NPG with Exact gradient

  [1] Agarwal et al. (2021)
  
  NPG ~ 1/epsilon^2.
    
  [2] Cen et al. (2020)
  
  NPG + regularization term add to the objective ~ linear rate.
  
  [3] Lan (2021)
  
  Policy mirror descent ~ linear rate (with regularization) or 1/epsilon (without regularization).
  
  [4] Khodadadian et al. (2021)
  
  NPG + adaptive stepsize ~ linear rate.
    
### Iteration complexity for Tabular + PG with Exact gradient
  [5] Bhandari and Russo (2021)
  
  PG + exact line search ~ linear rate. (The rate hide the infinity norm of d over u)
  
  [6] Mei et al. (2021)
  
  Geometric aware Normalized PG ~ linear rate. (The rate also hide the above term)
    
### Sample complexity for Tabular + NPG with approximate gradient
  [1] Agarwal et al. (2021)
    NPG (rollout estimation) ~ Sample complexity 1/epsilon^5
  [2] Cen et al. (2020)
    NPG + regularization term (rollout estimation) ~ 1/epsilon^2 (The dependence on 1/(1-gamma) is far from tight).
    
### General function approximation
  [1] Agarwal et al. (2021)
    Needs to make some assumption such as A^\pi(s,a) is almost linear in feature \nabla \log(\pi(a|s)).
