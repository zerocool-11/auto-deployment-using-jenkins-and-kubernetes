# auto-deployment-using-jenkins-and-kubernetes

## it will test the website feature automatically whenever developer push any new update for the website

### so here's the steps for doing this

#### i made 4 jobs for this task
* job1 - to get the data from github
* job2 - after this launching a deployment using yml file
* job3 - testing the app
* job4 - mailing the dev if the code isn't working

#### job 1
 it will pull the data from github whenever dev push any new update to the github
 
