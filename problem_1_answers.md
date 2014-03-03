1.

(a) Calender map visualization

Intended audience?
The intended audience for this visualization are visitors who are trying to get a bird's eye view of how active the user is on GitHub. This can be anyone in the user's social circle or potential recruiters who are trying to guage how involved the person is with open source projects. 

What data has been used and how you can you get it using the GitHub API?
Data on when and how many commits were done to the repository has been used. The data can be obtained using GET /users/:user/events for the Github API.

What happens if a contributor pushes many commits in a short time interval? How would you address this particular issue?
If many commits are pushed at the same time the color for the day on which these commits are pushed would become darker in color indicating increased activity.


(b) Contributors visualization

Intended audience?
The intended audience in this case would be people who are collaborating in the open source project. Potentially project mangers who are trying to asses who was most influential in the making of the project, may be when deciding on promotions. Also for the general public who care about the an open source community and want to see who is behind it. 

What data has been used and how can it be obtained using the Github API?
Data about how many commits were done by each author over a period of time has been used. It can be obtained using GET /repos/:user/:repo/commits from the Github API.

What happens if a contributor pushes many commits in a short time interval? How would you address this particular issue?
If many commits are pushed at the same time, the graph for the user pushing the commits would go up. The graph of overall commits will also go up.


(c) Commits visualization

Intended audience?
This visualization is likely intended for someone who wants to get details about the activity over the repository as the whole week progresses. Potentially project managers looking for info on what day of the week is most productive for developers. Or visitors trying to guess whether an open source project has corporate backing in which case most of the activity would be between work hours.

What data has been used and how can it be obtained using the GitHub API?
Data on when each of the commits to the repository were made. It can be obtained using GET /repos/:repo/commits.

What happens if a contributor pushes many commits in a short time interval? How would you address this particular issue?
The bar chart for that week would rise sharply and the line plot will have a point that is very high potentially requiring a change in the axis to be displayed properly.

(d) Code Frequency Visualization

Intended audience?
This is intended for developers who might want to look at when most of the addition and deletions of features occurred during the development process.

What data was used and how can it be obtained using the GitHub API?
Data on when each of the commits to the repository were made. It can be obtained using GET /repos/:repo/commits.

What happens if a contributor pushes many commits in a short time interval? How would you address this particular issue?
The graph grows in the positive or negative direction depending on the number of files that were added and deleted as a result of the commits.

(e) Punch Card Visualization

Intended audience?
This is intended for project managers trying to guage when developers are going to be the most productive so that they can make the environment more conducive to work during those hours.

What data was used and how can it be obtained using the GitHub API?
Again, the data on commits was used. It can be obtained using: GET /repos/:repo/commits.

What happens if a contributor pushes many commits in a short time interval? How would you address this particular issue?
The circle that represents the time of these commits would grow bigger than the other ones indicating the increased activity at that time. 

(f) GitHub Network Graph Visualizer

Intended audience?
This is intended for a wide range of audience including developers, project managers and general viewers. Basically anyone interested in getting a bird's eye view of the whole project and how the all the different branches work together.

What data was used and how can it be obtained using the GitHub API?
Data on the times of the different commits was used which can be obtained using: GET /repos/:repo/commits. Data on how many branches there are would also be useful and can be obtained using: GET /repos/:repo/branches

What is the role of interaction for this visualization? Would a static visualization have worked?
The visualization allows us to scroll from one point in time to the other and also shows the author info and the commit message when we hover over one of the commit dots. The scrolling allows us to fit long time intervals in the visualization which would not have been possible if it was static. The mouse over effect provides important information about the commit with he commit message. This is very helpful in tracking what kind of changes are being made in the repository.

What happens if suddenly a contributor pushes many commits in a short time interval? How would you address this particular issue?
There will be a lot of commit dots at the same place relative to each other which will make distinguishing them difficult. I would solve this by changing the scale of part of the visualization depending on the number of commit dots that need to be plotted.

