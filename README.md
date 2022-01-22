# eks-pipeline

Pipeline to do deployment on EKS cluster using jenkins, based on the envornment selected.

Assumptions :

You have already eks cluster and jenkins installed.

Steps 1: 
=======

Create a role using which ec2 instance can generate the kubeconfig file of eks cluster and assing it to jenkins server.

Step 2:
=======

Create parameterized pipeline as below :

