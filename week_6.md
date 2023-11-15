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

### AWS CodePipeline

AWS CodePipeline is a continuous integration and continuous delivery service for fast and reliable application and infrastructure updates. CodePipeline builds, tests, and deploys your code every time there is a code change, based on the release process models you define..


- [AWS Codecommit](https://docs.aws.amazon.com/codecommit/latest/userguide/getting-started-topnode.html) AWS CodeCommit is a fully-managed source control service that makes it easy for companies to host secure and highly scalable private Git repositories. CodeCommit eliminates the need to operate your own source control system or worry about scaling its infrastructure
  
- [AWS Artificats](https://docs.aws.amazon.com/codeartifact/latest/ug/getting-started.html) AWS CodeArtifact is a fully managed artifact repository service that makes it easy for organizations of any size to securely store, publish, and share software packages used in their software development process.
  
- [AWS CodeBuild](https://docs.aws.amazon.com/codebuild/latest/userguide/getting-started.html) AWS CodeBuild is a fully managed continuous integration service that compiles source code, runs tests, and produces software packages that are ready to deploy. With CodeBuild, you don’t need to provision, manage, and scale your own build servers. CodeBuild scales continuously and processes multiple builds concurrently, so your builds are not left waiting in a queue.
  
- [AWS CodeDeploy](https://docs.aws.amazon.com/codedeploy/latest/userguide/getting-started-codedeploy.html) AWS CodeDeploy is a fully managed deployment service that automates software deployments to compute services such as Amazon EC2, AWS Lambda, and your on-premises servers. AWS CodeDeploy makes it easier for you to rapidly release new features, helps you avoid downtime during application deployment, and handles the complexity of updating your applications.


![AWS CodePipeline](https://github.com/rcacfs/Project_Alpha/assets/24573829/8ed2e5d2-aa22-4a54-a542-142493cf0e87)

#### Tasks

##### Presequisite steps
- Have an already runnning EC2 instance with your EC2
- Create an S3 bucket for your application
- A code Reposiroty (github where your Source code is stores)

#### Steps

- Source Stage. This is where your source code resides either from - Github, gitlab, bitbucket and Codecommit
  - Create a version-controlled repository 
  - Developers clone the repository to their local machines for code contribution.
  - Developers write and modify the source code within their local copies of the repository.
  - Changes are committed to the version control system, ensuring a history of modifications.
  - Developers collaborate by pulling and pushing changes to and from the central repository.
  - Code reviews may be conducted to maintain code quality and catch potential issues early.
  
- Build Stage: In this stage, your source code is compiled, and any necessary dependencies are resolved. The result is a deployable artifact, such as an executable file or a package.
  - Set up a build configuration file that defines how the code should be compiled.
  - Specify dependencies and build instructions.
  - Whenever changes are pushed to the repository, trigger the automated build process.
  - The build server fetches the latest code, compiles it, and generates a deployable artifact.
  - The build process results in an artifact, such as an executable file, a library, or a packaged set of files.
  
- Test Stage: The deployable artifact goes through various tests to ensure that it meets the required quality standards. This can include unit tests, integration tests, or any other testing procedures you define.
  - Define a testing strategy, including unit tests, integration tests, and any other relevant test types.
  - Set up testing frameworks and environments.
  - Execute automated tests on the generated artifact to ensure it meets quality standards.
  - Tests may include checking functionality, performance, security, and other criteria.
  - Developers receive feedback on test results.
  - If issues are identified, developers iterate on the code, addressing and fixing problems.

- Deploy Stage: Once the code has passed all the tests, it is deployed to your target environment, whether it's a development, testing, or production environment.
  - Set up target environments for deployment, such as development, testing, and production environments.
  - Configure environment-specific variables.
  - Use deployment tools to automate the deployment process.
  - Deploy the artifact to the target environment.
  - Monitor the deployment for any issues or anomalies.
  - Validate that the deployed application functions correctly in the target environment.
  - Document the changes introduced in the deployment.
  - Communicate release notes to stakeholders.


### References

- [Redhat: What is CI/CD ](https://www.redhat.com/en/topics/devops/what-is-ci-cd)

- [Gitlab: CI/CD Explained ](https://about.gitlab.com/topics/ci-cd/)

- [AWS Codepipine](https://aws.amazon.com/codepipeline/product-integrations/?nc=sn&loc=6)

- [AWS Code Pipeline Intergrations](https://docs.aws.amazon.com/codepipeline/latest/userguide/integrations-action-type.html#integrations-source)

- [Youtube AWS Codepipeline Explained](https://www.youtube.com/watch?v=E5qjYTxVKvw)

- [Youtube Building an AWS Cloudpipeline](https://www.youtube.com/watch?v=8jml8Ni5cIE)

- [K12 Academy Deploy a web application using AWS Codepipeline](https://k21academy.com/amazon-web-services/aws-devops/deploy-web-application-on-aws-using-codepipeline/)



