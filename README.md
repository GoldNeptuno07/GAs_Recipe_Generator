# Recipes Generator 
### Genetic Algorithm

Given an amount of __calories__, the model will provide several __recipes__ that fit the amount given. Using a data base stored in a csv file, this model select random samples based on the 'n_genes' number provided by the user.


In this model I implement a roulette selection and a method to create the population, this method consists in pick a random point between 1 and (n_cromosomas) - 1 to split the father and mother and make mix, generating two samples. Note: If you want, you can modify this parameter to make it static instead of stochastic.


In addition, I implement a custom method to handle overfitting or underfitting, the details are in the code below.


You can play with the next parameters to reach your goal:
 * __calories__
 * __n_genes__
 * __n_cromosomas__
 * __split_point__
 * __overload_underload__
 
 
 __Note:__ Is important not to exceed the amount of ingredients stored in 'file.csv' with the parameters **n_genes** * **n_cromosomas** in this case not greater than __1070__.
 
__Issues__: At the end of the training step, the recipes could be duplicated and therefore the 'n' recipes can be halved.