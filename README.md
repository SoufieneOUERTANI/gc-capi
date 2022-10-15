To describe gc oprtions and parameters

https://www.baeldung.com/jvm-parameters

javac .\References.java
java -Xlog:gc .\References.class

PS D:\Learn\commit\gc> java -Xlog:gc\* .\References.class
[0.014s][info][gc,heap] Heap region size: 1M
[0.028s][info][gc ] Using G1
[0.029s][info][gc,heap,coops] Heap address: 0x0000000702800000, size: 4056 MB, Compressed Oops mode: Zero based, Oop shift amount: 3  
Error: Could not find or load main class .\References.class
Caused by: java.lang.ClassNotFoundException: /\References/class
[0.259s][info][gc,heap,exit ] Heap
[0.260s][info][gc,heap,exit ] garbage-first heap total 260096K, used 1024K [0x0000000702800000, 0x0000000800000000)
[0.260s][info][gc,heap,exit ] region size 1024K, 2 young (2048K), 0 survivors (0K)
[0.261s][info][gc,heap,exit ] Metaspace used 5065K, capacity 5127K, committed 5376K, reserved 1056768K
[0.262s][info][gc,heap,exit ] class space used 424K, capacity 429K, committed 512K, reserved 1048576K
