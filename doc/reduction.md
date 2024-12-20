# reduction


## example

count saturate summarization
```
const N = 5;
type element_t = logic<7>;

let a0 : element_t[N] = {43, 73, 3, 43, 80};
var o0 : element_t;

inst accumulator_7bit : reduction::<N, element_t, binop_satadd>(
    a: a0, 
    o, o0, // -> 127
);


```