# Concrete_Compressive_Strength
Introduction : Compressive strength is the ability of a material to withstand axial or compressive forces without failure. 
 It is usually measured by applying a compressive load to a standard cylindrical specimen until it breaks, 
 and then dividing the load by the cross-sectional area of the specimen. The compressive strength of concrete
 depends on various factors, such as amount of cement,coarse and fine aggregates, slag, superplastics(enhance setting rate)...

Dataset : It consists of 8 independent variables(all contunious) based on them we have to predict the strength(target
variable). There are 1000 rows with no missing values but Outliers were present.

Data-Preprocessing & EDA: Outlier treatment is performed and all variables are normally distributed after treatment.
 visualization using boxplots and dist plots has been done.

Model building : To detect multicollinearity PCA has been performed and 2 highly correlated varibles were removed.
XG Boost is the best performing model wit 87% R2 Score. 
More than 10 models have been used with the dataset ,Hyper parameter tuning with 10 fold cross validation has been 
performed to ensure the model does not overfit.

K-Means clustering is performed to visualize  the relationships with scatterplots and then grouped(target) with cement,
additonal features were created and the accuracy was improved to 90%.

Features importance with XG Boost gave Age, cement were most important one.
