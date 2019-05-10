## Set up new Repository

####Determine what to name the repository
- We have been using constellation names for our repositories and trying to find a constellation name that somehow matches the purpose of the repo
- We have a naming convention of [constellation]-web for a front-end project, [constellation]-data for a service layer (that has a front-end) and [constellation]-worker tend to be ETL workers.
- There are a number of projects that do not have a "-something" are projects that do not have a counterpart

####Create the new repository
1) At github.com/KPMP click the New button
2) Fill in the repository name with the name you decided on above
3) Give the project an appropriate description so that outside viewers can understand the purpose of the project
4) Leave it marked as pulic
5) Decide whether to initialize it with a README (if you don't have anything useful to put in there to start, feel free to leave it out)
6) Pick an appropriate .gitignore
7) Click "Create Repository"

###Set up repo
1) Clone the repo to you local machine
2) Create a branch named 'develop'
3) Make a small change, commit and push

###Set up contributors
1) Back on github, click the Settings icon in the upper right
2) Click on Collaborators & teams
3) In the "Teams" section click "Add a team" at the bottom
4) Select kpmp-dvc-admins
5) Change from Read to Admin 

###Set up branch rules
1) Under the Settings  in github select the "Branches" section
2) Change the default branch to develop
3) Click Add Rule
4) In "Branch Name Pattern" type develop
5) In Rule Settings check the "Require pull request reviews before merging" rule and click Create
6) Repeat for the master branch


