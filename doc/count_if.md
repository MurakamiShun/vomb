# count_if


## example

count less or equal 
```
const N = 5;
type element_t = logic<32>;

let a : element_t[N] = {43, 73, 3, 433, 80};
let b : element_t[N] = {84, 56, 4, 43 , 80};

var o : logic<$clog2(N+1)>;

inst count_less_eq : count_if::<N, logic, predop_less_eq>(
    a,
    b,
    o, // -> 3
);

```