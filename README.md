# eks-pipeline

Pipeline to do deployment on EKS cluster using jenkins, based on the envornment selected.

Assumptions :

You have already eks cluster and jenkins installed.

Steps 1: 
=======

Create a role using which ec2 instance can generate the kubeconfig file of eks cluster and assing it to jenkins server.

Step 2:
=======

Create new job "eks-deploy" of the type pieline.


![image](https://user-images.githubusercontent.com/74225291/150649928-d718051a-ecce-4ca0-9e0a-18593e3782c1.png)

Make this job as a parametrized and add two parameter "environment and aws-region"
Depending on the envirnment and region we can select the cluster.

![image](https://user-images.githubusercontent.com/74225291/150650016-f16fa73d-88e7-4081-88c1-1e238d404d66.png)


![image](https://user-images.githubusercontent.com/74225291/150650085-600e854e-1923-4af3-bbe8-1bd413887b82.png)

![image](https://user-images.githubusercontent.com/74225291/150650095-57c1c5f9-c3f1-42da-8947-7c8d258a0e5f.png)

Now past the jenkinsfile code in pipeline and save it.

And  build the job with parameter.


![image](https://user-images.githubusercontent.com/74225291/150650144-af9e5ee7-3f61-48ca-a897-e00aed1dbea9.png)

And check the output in console section.

Have attach output in console.log section.


