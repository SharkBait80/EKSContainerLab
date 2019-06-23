
# .NET Framework Application Modernization using .NET Core, Docker Containers, and Amazon EKS

Application modernization presents designers with a spectrum of technology migration options including:

* Do we retain the current monolithic application architecture?
* Shall we refactor the application architecture using a Cloud Native model?
* Given time and resource constraints, should we simply replatform the application using Virtual Machines?

Ultimately, a Container based solution can account for each of these modernization scenarios.  Legacy applications tend to exist in maintenance mode with few dedicated software development resources.  Hence retaining some or all of the existing solution architecture and rehosting via Containers or Virtual Machines may be the only viable first step.

A key consideration is to determine what solution elements cannot easily be refactored. Common .NET Framework application dependencies such as the Windows Registery, third-party libraries, file system APIs, IIS integrations, and data-access technologies, are now considered anti-patterns relative to Cloud Native architectures.


### TODO : ILLUSTRATE THE SOLUTION ARCHITECTURE AND AWS TECHNOLOGIES

 
### TODO : SPEAK TO THE LAB ENVIRONMENT INCLUDING WINDOWS AND LINUX WORKSTATION CONFIGURATION




### Begin the Workshop

[Proceed to Module 1](/module-1)


### Topical Agenda by Modules

* [Module 1 - Configure your Linux Dev Environment](/module-1)
* [Module 2 - Configure your EKS Cluster](/module-2)
* [Module 3 - Configure your Windows Server Dev Environment](/module-3)
* [Module 4 - Build the Sample .NET Framework Application](/module-4)
* [Module 5 - Transform the Sample Application to .NET Core](/module-5)
* [Module 5 - Dockerize the Sample Application ](/module-5)
* [Module 6 - Deploy the Sample Application to your EKS Cluster](/module-6)
* [Module 7 - title](/module-7)


### Workshop Clean-Up (Once Complete)
Be sure to delete all of the resources created during the workshop in order to ensure that billing for the resources does not continue for longer than you intend.  We recommend that you utilize the AWS Console to explore the resources you've created and delete them when you're ready.

For the any cases where you provisioned resources using AWS CloudFormation, you can remove those resources by simply running the following commands for each stack:

__AWS CLI__
```
aws cloudformation delete-stack --stack-name STACK-NAME-HERE
```

To remove all of the created resources, you can visit the following AWS Consoles, which contain resources you've created during this workshop:

* [AWS Lambda](https://console.aws.amazon.com/lambda/home)
* [Amazon S3](https://console.aws.amazon.com/s3/home)
* [Amazon EC2](https://console.aws.amazon.com/ec2/home)
* [Amazon VPC](https://console.aws.amazon.com/vpc/home)
* [AWS IAM](https://console.aws.amazon.com/iam/home)
* [AWS CloudFormation](https://console.aws.amazon.com/cloudformation/home)


[Proceed to Module 1](/module-1)


## [AWS Developer Center](https://developer.aws)






















