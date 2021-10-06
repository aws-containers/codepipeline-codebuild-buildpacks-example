# AWS CodePipeline & AWS CodeBuild with Cloud Native Buildpacks

Pipeline that demonstrates how to integrate Cloud Native Buildpacks with AWS tools. Please see this [blog post](https://aws.amazon.com/blogs/containers/creating-container-images-with-cloud-native-buildpacks-using-aws-codebuild-and-aws-codepipeline/) for details on how it can be used.

This pipeline uses AWS DevOps tools AWS CodeCommit, AWS CodePipeline, AWS CodeBuild and Amazon Elastic Container Registry (ECR) along with other AWS services.

The file `cloudformation.yml` contains all of the AWS CloudFormation necessary to deploy the solution, including:
- CodeCommit repository
- ECR repository
- CodeBuild project to build the container image
- CodePipeline to orchestrate code checkout and running CodeBuild
- Lamba function and custom resource to seed the CodeCommit repository with a sample Spring Boot application

## Deploying pipeline:
Download the CloudFormation template and pipeline code from GitHub repo.

1.	Log in to your AWS account if you have not done so already. 
2.	On the CloudFormation console, choose Create Stack. 
3.	Choose the provided CloudFormation pipeline template. 
4.	Choose Next.

## License

Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
SPDX-License-Identifier: MIT-0
