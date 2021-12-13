## tuning GC

* [for latency](https://docs.oracle.com/javase/9/gctuning/garbage-first-garbage-collector-tuning.htm#JSGCT-GUID-4914A8D4-DE41-4250-B68E-816B58D4E278)
  * `-XX:MaxGCPauseMillis=10` (defaults to `200ms`) 
  * `-Xms=-Xmx` + `-XX:+AlwaysPreTouch` to prevent (de)allocation to/from OS
* [for throughput](https://docs.oracle.com/javase/9/gctuning/garbage-first-garbage-collector-tuning.htm#JSGCT-GUID-70E3F150-B68E-4787-BBF1-F91315AC9AB9)
