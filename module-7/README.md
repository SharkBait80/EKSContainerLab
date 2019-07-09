# Module 7 - Deploy the Sample Application to your EKS Cluster


**Time to complete:** 20 minutes

**Services used:**

- Elastic Container Registry (ECR)

- Elastic Kubernetes Service (EKS)

### Overview

From the previous module, you should have obtained a Docker image that you are ready to push to ECR (Elastic Container Registry). [Amazon ECR](https://aws.amazon.com/ecr/) is a fully-managed Docker container registry that makes it easy for developers to store, manage, and deploy Docker container images.

Follow the [instructions here](https://docs.aws.amazon.com/AmazonECR/latest/userguide/docker-push-ecr-image.html) to login, tag and push your Docker image to ECR.

Once you have pushed your image to ECR, you can deploy it to your EKS cluster that you setup in module 2. Kubernetes supports ECR as a private repository, [as detailed here](https://kubernetes.io/docs/concepts/containers/images/#using-aws-ec2-container-registry).

To deploy your image onto EKS, use the "kubectl run" command, passing in the name of your application and the URL to your image in ECR.


## Next

Please proceed to the next lesson.

**[Proceed to Module 8](/module-8)**


### [AWS Developer Center](https://developer.aws)
