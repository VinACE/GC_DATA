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
