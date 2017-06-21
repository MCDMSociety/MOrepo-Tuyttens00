# Bicriterion linear assignment problems

The paper consider 10 instances for the classical bi-objective linear assignment problem. 

## Test instances

Instances are named `Tuyttens_AP_n<n>.<raw/xml>` where `n` is the size of the problem. The paper considers
instances of size 5-50; however, the instance set also contains 5 instances of size 60-100. Costs
are generated random in [0,19].

All instance files are given in both xml and raw format. The xml format is self explainable (see
e.g. [ex1](./instances/xml/Tuyttens_AP_n05.xml)).


### Raw format description

We use the following parameter names:

* $n$ = dimension/size
* $c^{k}_{r,c}$ = $k$'th cost of assigning row $r$ to column $c$.

The instances have the following format:

```
n 
c^{0}_{0,0}... c^{0}_{0,n-1}
c^{0}_{1,0}... c^{0}_{1,n-1}
...
c^{0}_{n-1,0}... c^{0}_{n-1,n-1}
c^{1}_{0,0}... c^{1}_{0,n-1}
c^{1}_{1,0}... c^{1}_{1,n-1}
...
c^{1}_{n-1,0}... c^{1}_{n-1,n-1}
```

That is, first the dimension, then the costs for the first criterion and next the cost for the
second criterion.











