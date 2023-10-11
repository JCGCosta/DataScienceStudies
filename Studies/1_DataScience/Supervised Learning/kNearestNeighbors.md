The kNearestNeighbors is an algorithm in the supervised learning used to classification and regression, the problem can be describe as: imagining a labeled dataset with different clusters, then a new instance show up, and we need to classify that instance, the knn will classify that instance based on the **k** nearest instances, by plurality vote. 

![[Pasted image 20230927101411.png]]

In the example above for k=3 the knn will classify that instance as 'class B' because there the majority class appearance is 'class B', otherwise for k=7 the instance will be classified as 'class A', also because the 'class A' is the majority in that scenario.