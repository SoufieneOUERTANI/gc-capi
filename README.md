To describe gc oprtions and parameters

https://www.baeldung.com/jvm-parameters

javac .\References.java

PS D:\Learn\commit\gc> java -Xlog:gc References
[0.040s][info][gc] Using G1
aref has a reference to object : first-last
dref has a reference to object : first-last
eref has a reference to object : start-end
---------Finally-------------
aref has a reference to object : null
bref has a reference to object : start-end
dref has a reference to object : start-end
dref has a reference to object : null
eref has a reference to object : start-end

PS D:\Learn\commit\gc> java -Xlog:gc\* References
[0.016s][info][gc,heap] Heap region size: 1M
[0.030s][info][gc ] Using G1
[0.031s][info][gc,heap,coops] Heap address: 0x0000000702800000, size: 4056 MB, Compressed Oops mode: Zero based, Oop shift amount: 3  
aref has a reference to object : first-last
dref has a reference to object : first-last
eref has a reference to object : start-end
---------Finally-------------
aref has a reference to object : null
bref has a reference to object : start-end
dref has a reference to object : start-end
dref has a reference to object : null
eref has a reference to object : start-end
[0.230s][info][gc,heap,exit ] Heap
[0.231s][info][gc,heap,exit ] garbage-first heap total 260096K, used 2048K [0x0000000702800000, 0x0000000800000000)
[0.232s][info][gc,heap,exit ] region size 1024K, 3 young (3072K), 0 survivors (0K)
[0.233s][info][gc,heap,exit ] Metaspace used 4980K, capacity 5062K, committed 5120K, reserved 1056768K
[0.233s][info][gc,heap,exit ] class space used 424K, capacity 458K, committed 512K, reserved 1048576K
PS D:\Learn\commit\gc>
