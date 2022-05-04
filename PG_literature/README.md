### Iteration complexity for Tabular + softmax parameterization with NPG with Exact gradient

  [1] Agarwal et al. (2021)
  
  NPG = iteration complexity $O(\frac{1}{(1-\gamma^2 \epsilon)})$.
    
  [2] Cen et al. (2020)
  
  NPG + regularization term add to the objective = iteration complexity $\frac{1}{1-\gamma}\log(\frac{1}{\epsilon})$.
  
  [3] Lan (2021)
  
  Policy mirror descent = linear rate (with regularization) or $O(\frac{1}{\epsilon})$ (without regularization).
  
  [4] Khodadadian et al. (2021)
  
  NPG + adaptive stepsize = linear rate.
    
# Iteration complexity for Tabular + PG with Exact gradient
  [5] Bhandari and Russo (2021)
  
  PG + exact line search = linear rate. (The rate hide the $\|\frac{d^{\pi^*}}{u}\|_\infty$ factor)
  
  [6] Mei et al. (2021)
  
  Geometric aware Normalized PG = linear rate. (The rate hide the $\|\frac{d^{\pi^*}}{u}\|_\infty$ factor)
    
# Sample complexity for Tabular + NPG with approximate gradient
  [1] Agarwal et al. (2021)
    NPG (rollout estimation) $\approx O(1/\epsilon^5)?$
  [2] Cen et al. (2020)
    NPG + regularization term (rollout estimation) $\sim O(\frac{|S||A|}{(1-\gamma)^8}\epsilon^2)$.
    
# General function approximation
  [1] Agarwal et al. (2021)
    Needs to make some assumption such as $A^\pi(s,a)$ is almost linear in feature $\nabla \log(\pi(a|s))$.
