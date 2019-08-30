# How to install metabase with  aws ecs docker fargate

1 Create your own cluster with a unique name with the following command :

  - ``` aws ecs create-cluster --cluster-name fargate-cluster-name ```

2. write $fargate-cluster-name ,$ACCOUNT_ID , $DB_ENDPOINT and $DB_PASSWORD

3.  JSON file for container definitions:

  - ``` aws ecs register-task-definition --cli-input-json file://$HOME/tasks/fargate-task.json ```

 ### Now our task is ready

 ### Create your Application Load Balancer and Target Groups

 #### Loadbalancer

 ![Alt text](img/img3.png?raw=true "Title")

 #### Target Group

 ![Alt text](img/img2.png?raw=true "Title")

 ### Create Security Groups

 	*  Security for postgresql Rds
 	*  Elb Security Groups
 	*  Create for Security Group for Application




##  Create Service

1. **Step** 


![Alt text](img/img.png?raw=true "Title")




2. **Step** 



![Alt text](img/img5.png?raw=true "Title")

![Alt text](img/img4.png?raw=true "Title")


3 **Step**


![Alt text](img/img6.png?raw=true "Title")



> If you have problems you can contact me at this website [Vmward](https://vmward.co.uk)



