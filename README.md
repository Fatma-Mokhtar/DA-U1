# DA-U1
my_vector_1<- c(1,2,3,4,5)
print(my_vector_1)
length(my_vector_1)

my_vector_2<-c(1:10)
print(my_vector_2)
length(my_vector_2)

my_vector_3<-c(10:5)
print(my_vector_3)
length(my_vector_3)

my_vector_4<-seq(from=0, to=30, by=10)
print(my_vector_4)
length(my_vector_4)

my_vector_1[1]
my_vector_2[1:3]
my_vector_3[c(1,3)]

my_vector_1[3]<-30
my_vector_4[c(2,3)]<- c(20,30)

my_added_vector<-c(my_vector_1[1:3],20,my_vector_1[4:length(my_vector_1)])
my_deleted_vector<-c(my_vector_1[1:3],my_vector_1[5:length(my_vector_1)])

my_short<-c(1,2,3)
my_long<-c(10,20,30,40,50,60)
my_sum<-my_short+my_long
print(my_sum)

##data frame

x<-c(2.5,3.5,3.4)
y<-c(5,10,1)
my_df<-data.frame(x,y)
print(my_df)

colnames(my_df)<-c('Floats','Integers')
my_other_df<-data.frame(X=c(2,3,4), Y=c('A','B','C'))
print(my_other_df)

ncol(my_other_df)
nrow(my_other_df)
str(my_other_df)

my_other_df[1,]
my_other_df[,2]
my_other_df$Y
my_other_df[c(1,3),]
head(my_other_df,2)
tail(my_other_df,3)


my_other_df$X[3]<-400
print(my_other_df)

my_other_df$X <- c('200','300','401')
print(my_other_df)
my_other_df[,1] <- c('200','300','402')
print(my_other_df)

my_other_df$Z<-c(255,300,100)
print(my_other_df)

my_other_df[,3]<- NULL
print(my_other_df)
