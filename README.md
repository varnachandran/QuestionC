# QuestionC
Assigning numbers to cities

For question c on assigning unique numbers to cities, the aim is to find the algorithm used to generate the sample output from the sample input given.
I was successfully able to generate unique numbers from strings, but unfortunately , I could not decode the algorithm used for the sample input output set.
I tried the following approaches:

1)All the letters in the English alphabet would be assigned unique weights, with some positive weights and rest negative weights(especially in the beginning of the alphabet).

The reason why I think there are negative weights is because for some words, the output value is very low and even negative.

2)The weights assigned to the letters should be added as powers of say 3 or 4.

But in that case, for the 2 works cork and york, all the letters except the first one are the same(even the positon of the letters)

So the polynomial coeffients should be the same for both the words except for the coefficients corresponding to c and y.

this made me conclude that y-c=4426-246=4180

But even in this case none of the conditions are true:


1)the sum of cubes of any 2 numbers =4180

2)The difference of cubes of any 2 numbers =4180 

3)the sum of power of 4 of any 2 numbers =4180

4)The difference of power of 4 of any 2 numbers =4180 


y or c cannot be power of 1, in that case the y-c would have been very small value. they can also not be power of 5 or more too


3)I also assigned positive coefficients to letters in even positions and negative for letters in odd positions, that does not work either

4)Also tried positive value based on count from the letter 'a'. ie, for if the letters are 'ac' the sum is 2. if the letters are 'ca', sum is -2. The same logic did not work for powers of counts as well

5)Also tried to use machine learning algorithms using sci-kit learn, fit and predict . But that did not work either.

Also, the input sample set does not contain a word with the letter 'w', and it is not possible to get the output for the word 'naypyidaw'
