# Ж Process to solve DP Ж

## DP   Searching optimal Solution 

(1) **_Define subprobelms_** ▷  # of subproblems 

(2) **_Guess(part of solution)_** ▷  choices of guess

(3) **_Related subproblem solution_** ▷  time/subproblem

(4) **_Recurse & memoize_**   ▷  check subproblem recurrence is acyclic and has topological order

(5) **Solve the original problem**
# 

## ▶   Analyzation

### - make1.cpp
(1) # of subproblems    :   ϴ (n)

(2) choices of guess    :   bottom-up approach & pick the min value from table

(3) Recurrence formula  :   min(table[i/3], table[i/2], table[i-1])
    time/subproblem     :   ϴ (1)

(4) topological order   :   k = 1, 2, ···, n (ok)
                            total time = ϴ (n^2)
(5) Original Prob       :   DP(n) = ϴ (1) 

### -  sugar_delivery.cpp
(1) # of subproblems    :   N / 3 →  ϴ (n)

(2) Guess               :   find total count when # of 3kg is changed

(3) Recurrence          :   count 5kg when 3kg is changed 
                            subprob time : ϴ (1)

(4) Topological?        :   n, n-1, ··· 0
                            total time :ϴ (n) 

(5) Original Problem    :   min(DP_table)


