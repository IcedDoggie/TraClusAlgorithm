# TraClusAlgorithm

This is an implementation of TraClus [1] algorithm in Java. A GUI was added for the convenience.

The original paper of this algorithm can be found at http://hanj.cs.illinois.edu/pdf/sigmod07_jglee.pdf 
The authors of the paper implemented the algorithm in C++, so it could be helpful to develop one in Java for 
other users to use. I have compared the output with the one generated by the C++ implementation, so far I have not found
any bugs. It will be great if any one reports any bugs about this implementation.

I am currently involved in a maritime traffic project which requires me to implement various clustering algorithms. So that
is the very first motivation about why I do this implementation. I also implment another clustering algorithm called DBSCANSD
which is proposed during my thesis study and I will put it into the github later. 



How to run the code?

After downloading it to local, 
1. cd to the folder of src/boliu/
2. compile all the .java files using:
    javac *.java
3. cd to the folder of src/
4. execute the program using the following either commands:

    1) java boliu.Main inputfile outputfile eps minLns 
        --e.g. java boliu.Main deer_1995.tra testOut.txt
        In this way, the program will help you to decide the parameters for eps and minLns;

    2) java boliu.Main inputfile outputfile 
        --e.g. java boliu.Main deer_1995.tra testOut.txt 29 8
        In this way, you tell the program the parameters for eps and minLns, which are 29 and 8 seperately.

5. wating for the result :)





[1] Lee, Jae-Gil, Jiawei Han, and Kyu-Young Whang. "Trajectory clustering: a partition-and-group framework."
Proceedings of the 2007 ACM SIGMOD international conference on Management of data. ACM, 2007.


