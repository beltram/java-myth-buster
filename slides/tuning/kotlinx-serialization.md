## Use kotlinx.serialization

* generates AOT bindings ; does not require reflection like Jackson
* faster for json, slower for xml  

| ms/ops (lower is better)              |  avg  |  p90  |  p99  | 
|---------------------------------------|-------|-------|-------|
| jackson (deser)                       | 0.129 | 0.166 | 0.326 |
| kotlinx.serialization (deser)         | 0.028 | 0.030 | 0.074 |
| jackson (serialization)               | 0.017 | 0.019 | 0.046 |
| kotlinx.serialization (serialization) | 0.015 | 0.017 | 0.043 |
