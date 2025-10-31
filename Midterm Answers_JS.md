## Question 1.1 Answer:
The LASSO spaghetti plot above shows how the coefficients change as the penalty of alpha (lambda) changes. The optimal lambda is 0.0009 plotted as the vertical red dotted line. Each colored line represents a coefficient of X (e.g., attributes or genres).

The LASSO analysis is pushing weaker coefficients to 0 so that stronger coefficients can stand out from the noise. The optimal penalty as shown above from the cross validation chart will zero out multiple coefficients to leave only the strong ones for analysis. Below we will print some of the top coefficients to look at.

This chart of predictors shows that there are 45 active coefficients and the strongest positive predictors are 'black comedy', 'animation', and 'documentary' while the strongest negative predictors are 'horror', 'superhero', and 'children'

The story this analysis tells is effectively what the movie population likes and doesn't like from our dataset. For example, it would make sense Horror films typically don't get great ratings because many movie watchers including myself don't like the category at all. Similarly, negative predictors like 'politics' or 'adultery' are pretty obvious scenarios where the movies may miss the mark with a not as pleasing topic to the general public and therefore get worse ratings. Let's also look at the positive predictors. This is where we see some of the most liked types of movie attributes like black comedy which is a specific type of funny content people lvoe as well as emotional and drama which both are one of the largest movie categories for women right next to war, sci-fi, and western, which are probably also the top categories for men to watch.

Also, one thing to consider here is the way these movies make people feel. The positive predictors typically handle bold and resonating topics that are well liked for their higher engagement of people from all background. The negative predictors to contrast are more constrained to movie watchers that like that specific genre for instance boxing has a great following of people that love boxing yet doesn't appeal to everybody due to violence.

## Question 1.2 Answer:
What we see by the above calculations is that the penalty for lambda that gives us the best prediction will be 0.0009 which is the same as what we saw as the vertical red dotted line on the previous charts. This lambda leaves 45 active attributes/genres to contribute to prediction.

The smallest out of sample prediction error is shown above as MSE=0.25 which represents the mean squared error. This is the minimum average squared distance between the true ratings and the model's predicted ratings. To make it more meaningful we can take the square root which is about 0.50. This means the model will predict the movie ratings within about 1 point (0.50 up and 0.50 down) from the actual ratings. With this MSE value we want to observe the smallest number possible and this is sufficient in my opinion.

## Question 1.3 Answer:
By looking at a single slice out of the 10 slices we can see how the coefficients change due to sample differences (or hopefully overlap) especially to test if most of the coefficients still appear in the top 10.

For instance we see black comedy, documentary, and animation, again for positive predictors and horror, superhero and highschool for negative predictors. That's great! We also see some addiitonal nuances of the smaller sliace which adds imdb toip 250 or dark into the positive predictors when they weren't there previously. This just means in that specific slice those attributes become predictors of higher ratings, but then when incorporated into the whole model they slip out of the top 10

Another good thing to see is that the selected features remains 45 which means the model is relatively stable at the slice and whole level. 

## Question 1.4 Answer:
Looking back at the full model. Horror as an attribute had the coefficient = -0.3114 what this means is that if two movies had the exact same attributes but one had Horror and one did not, the horror movie would have a lower rating by 0.31 on the ratings scale. The awesome part about this analysis is that we can use the coefficients to say: all else equal, if a movie is horror and the other isnt than we can predict the horror movie to have lower 0.31 rating score.

Another way to consider this is looking at black comedy on the positive side. If two movies had identical attributes except one had black comedy and the other didn't then the black comedy movie we would preedict would have 0.28 higher points in the reviews simply for that attribute.

## Question 2.1 Answer:
Answer Here

## Question 2.2 Answer:
Answer Here

## Question 2.3 Answer:
Answer Here

## Question 2.4 Answer:
Answer Here

## Question 2.5 Answer:
Answer Here

## Question 2.6 Answer:
Answer Here

## Question 2.7 Answer:
Answer Here

## Question 2.8 Answer:
Answer Here

## Question 3 Answer:
Answer Here