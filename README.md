GC_DATA
=======

getting and cleaning Data Exercise

This is to perform the basic operation of merging the test and train data set.

dataset1 = read.table("X_test.txt", sep="\t")

dataset2 = read.table("X_train.txt",sep="\t")

merged.data.all <- merge(dataset1, dataset2, by="V1", all.x=TRUE)

dataset3 = read.table("body_acc_x_test.txt", sep="\t")

dataset4 = read.table("body_acc_x_train.txt",sep="\t")

merged.data.acc <- merge(dataset3, dataset4, by="V1", all.x=TRUE)
### subsetting the combined data set.X

X <- data.frame("V1" = sample(1:5))
X <- data.frame("V1" = sample(1:5),"v2"=sample(1:5))

 > X <- data.frame("V1" = sample(1:5),"v2"=sample(1:5))  smalll subset operation..
> X
  V1 v2
1  1  4
2  5  5
3  3  3
4  4  1
5  2  2
> 

### Tail of merged data... showing 2947 rows hence the data is merged.

> tail(merged.data.acc,1)                                                                                                                                                                                                                                                                                                                                                         V1
2947   9.9997130e-003  1.1399670e-002  1.2362370e-002  9.6387010e-003  7.0903970e-003  9.0608340e-003  1.2125240e-002  1.3123010e-002  1.2419780e-002  7.9527940e-003  2.7967950e-003  4.2183640e-003  6.1402580e-003  5.3893080e-003  7.6344450e-003  7.4963530e-003  4.9400930
