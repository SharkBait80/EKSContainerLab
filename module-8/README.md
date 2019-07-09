# Module 8 - Test Your Application on EKS


**Time to complete:** 20 minutes

**Services used:**

- Elastic Container Registry (ECR)

- Elastic Kubernetes Service (EKS)

- Simple Storage Service (S3)

### Overview

In this module, we will test our application to check if it is running properly on our EKS cluster.

In order to check application output, you can view the logs from pods.

To get the name of the pods running on your nodes, use the "kubectl get pods" command.

Pass the name of the pod into the "kubectl logs" command to see the output.

### Defining arguments

To test our application properly, we'd want to pass in the same arguments as we did when the application was running on our local machine.

Create a YAML file that specifies the path to the text file with the input VLAN IDs.

~~~~

apiVersion: v1
kind: Pod
metadata:
  name: command-demo
  labels:
    purpose: demonstrate-command
spec:
  containers:
  - name: command-demo-container
    image: <Your ECR image path>
    command: ["dotnet"]
     args: ["-f", "TEST-DATA/SampleVLANs.txt","-e",TEST-DATA/Exceptions0001.log","-o","TEST-DATA/Router001.txt","-p","TEST-DATA/Router002.txt"]
  restartPolicy: OnFailure

~~~~

Upload this file as command.yaml to an S3 bucket, and allow it to be accessed from the Kubernetes pods.

Create a Pod based on the YAML configuration file:

kubectl apply -f INSERT_URL

Once the pod has been created, you can inspect the logs by running

_kubectl logs command-demo_

You should now see the program output, just as if you were running it locally.

## Next

### Congratulations, You have successfully completed the migration of a .NET application and deployed it onto EKS.


### [AWS Developer Center](https://developer.aws)