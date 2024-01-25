## Annotations-to-Datacamp-R-skills
# My annotations to Datacamp R Skills to help me remember important coding hints. 

#Parentheses are not placed around Logic variables 
#eg 
Boolean_Vector <- (TRUE, FALSE, TRUE) #not ("TRUE", "FALSE", "TRUE")

#No parentheses to assign a variable under operator names

**Assign the names of the day to roulette_vector and poker_vector**
names(poker_vector) <-  days_vector
names(roulette_vector) <- days_vector

**checking comparison of vector elements is simple** 
**Which days did you make money on poker?**
selection_vector <- poker_vector > 0

**logic vector in square brackets selects elements that are TRUE of the original vector**
**dimnames = list(titles, region) this is the format for dimnames . Remember list.** 

**Do not use parentheses in Square brackets to reveal members**
planets_df[positions, ]

**when naming lists remember name comes first then list member**
**no parentheses** 
my_list <- list( vec = my_vector, mat = my_matrix, df = my_df)

**sum function on logical vectors calculates number of TRUE's.**
**very important use args(sd) for eg to find arguments of a function in R**
Remeber this template for function creations. 
my_fun <- function(arg1, arg2) {
  body
}




**For Loop**
for ( i in 1:length(cities)) {
print(paste(cities[i], "is on position", i , "in the list" ))
}

# Notice that you need double square brackets - [[ ]] - to select the list elements in for loop version 2.
