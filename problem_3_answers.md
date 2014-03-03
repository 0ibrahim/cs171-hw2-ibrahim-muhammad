Given your previous design critiques, your experience with the previous graph visualization implementation and the reading of the article cited below (Lee et al., 2006), answer the following questions:

Which graph-related tasks does an ideal GitHub Network Graph need to address?

> The ideal GitHub graph will neeed to show us how the differnt branches of the repository interact together, which repository was forked from which and whih was it merged with. It should constitute a holistic overview of code commiting history by differnt contributors. Individual commits are not as important as showing how the code developed over the different repositories in the time that  we are tracking.

Get back to the GitHub network visualization you implemented and test it with the following projects on GitHub: D3, jQuery and Bootstrap. There's a lot more data, but the interaction patterns of users are also very different. What do you notice about the three repositories?

>It appears D3's development was largely driven by one person who was committing to a single branch. After some time new people started joining the efforts and it became more popular. It also shows that the development slowed down in the middle and then picked up again.

>jQuery's development was faster compared to d3 and it was also a result of more people being involved at more or less the same rate.

>Bootstrap's development was also more or less driven by one or two people who were commiting code regularly. It seenms the pace of development was pretty uniform except for a break or two in between. 


How does this impact your graph?
>At times by graph shows too many points at a single time so it is difficult to distinguish  between them. At times some of the points go outside the graph due to the large volume of the data.


How would you improve your visualization to address issues with the larger and more complex data?
>In case there are too many commits at the same time. I would like to blob them together and represent the collection of commits as a single circle but with proportional area. By doing this we can better appreciate the number of commits that happened at the same time.

> I would also want to change the scales when the data is too large so that no stray points go outside.
