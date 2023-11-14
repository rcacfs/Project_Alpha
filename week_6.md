# Week 6 - CI/CD 

## What is CI/CD
CI/CD falls under DevOps (the joining of development and operations teams) and combines the practices of continuous integration and continuous delivery. CI/CD automates much or all of the manual human intervention traditionally needed to get new code from a commit into production, encompassing the build, test (including integration tests, unit tests, and regression tests), and deploy phases, as well as infrastructure provisioning. With a CI/CD pipeline, development teams can make changes to code that are then automatically tested and pushed out for delivery and deployment. Get CI/CD right and downtime is minimized and code releases happen faster.

### CI/CD Tools

Popular CI/CD tools that can help you achieve your objectives

- [AWS CodePipeline](https://aws.amazon.com/codepipeline/) AWS CodePipeline is a fully managed continuous delivery service that helps you automate your release pipelines for fast and reliable application and infrastructure updates

- [Github Actions](https://docs.github.com/en/actions) GitHub Actions is a continuous integration and continuous delivery (CI/CD) platform that allows you to automate your build, test, and deployment pipeline
  
- [Jenkins](https://www.jenkins.io/) Jenkins is an open-source automation server in which the central build and continuous integration process take place.
  
- [Circle CI](https://circleci.com/) CircleCI is a CI/CD tool that supports rapid software development and publishing. CircleCI allows automation across the user’s pipeline, from code building
  
- [Gitlab](https://about.gitlab.com/) GitLab is a suite of tools for managing different aspects of the software development lifecycle.

### Tasks

The tool that will be used for the deployment is AWS Codepipeline

![AWS CodePipeline](https://github.com/rcacfs/Project_Alpha/assets/24573829/8ed2e5d2-aa22-4a54-a542-142493cf0e87)

#### Tasks

- Source Stage. This is where your source code resides either from - Github, gitlab, bitbucket and Codecommit
  
- Build Stage: In this stage, your source code is compiled, and any necessary dependencies are resolved. The result is a deployable artifact, such as an executable file or a package.
  
- Test Stage: The deployable artifact goes through various tests to ensure that it meets the required quality standards. This can include unit tests, integration tests, or any other testing procedures you define.

- Deploy Stage: Once the code has passed all the tests, it is deployed to your target environment, whether it's a development, testing, or production environment.



### References

- [Redhat: What is CI/CD ](https://www.redhat.com/en/topics/devops/what-is-ci-cd)

- [Gitlab: CI/CD Explained ](https://about.gitlab.com/topics/ci-cd/)

- [AWS Codepipine](https://aws.amazon.com/codepipeline/product-integrations/?nc=sn&loc=6)

- [AWS Code Pipeline Intergrations](https://docs.aws.amazon.com/codepipeline/latest/userguide/integrations-action-type.html#integrations-source)

- [Youtube AWS Codepipeline Explained](https://www.youtube.com/watch?v=E5qjYTxVKvw)

- [Youtube Building an AWS Cloudpipeline](https://www.youtube.com/watch?v=8jml8Ni5cIE)




