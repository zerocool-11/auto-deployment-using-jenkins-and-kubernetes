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
![alt text](https://github.com/zerocool-11/auto-deployment-using-jenkins-and-kubernetes/blob/master/images/git-task-3.png) 


#### job 2
 it will get trigger after the successful execution of job 1 for this job i made 2 type of yml file 
 1. for php
 2. for html
 so it the code is for php it will launch the dep for php type code using one custom php image and same for html
![alt text](https://github.com/zerocool-11/auto-deployment-using-jenkins-and-kubernetes/blob/master/images/task-3-dep.png)

#### job 3
this will test the code using curl   if the testing fails job 4 will get triggered which will mail the developer
![alt text](https://github.com/zerocool-11/auto-deployment-using-jenkins-and-kubernetes/blob/master/images/task-3-testing.jpg)

### Here's the full pipeline view of this project
![alt text](https://github.com/zerocool-11/auto-deployment-using-jenkins-and-kubernetes/blob/master/images/task-3-view.jpg)

