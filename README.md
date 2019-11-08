# Cloud Devops Project 3: Create a pipeline with Jenkins

## Achievement
* Nov 1, 2019, submitted to review in Udacity and passed.

## Todo


* I need to delete my ec2 instance and s3 bucket as soon as I decide to do it.

* Blue/Green deployment
* canary deployment
* phasing out deployment
* github push to build server


* The Jenkinsfile can be extended easily, we added a linting stage, other steps can be added like ensuring content is up with a curl command.
* “Steps” have useful features like a ‘retry’, anything that can be added to make it a robust deployment is great. See the reference guide.
* The project was created with a “poll” to check for Github changes. A webhook can be added instead that makes Github tell Jenkins to start building automatically. Github has a good guide on how to do this.
* Another option that can be done is using Canary Deployments. A Canary deployment is a more involved setup, and would require to progressively route users to the new version deployed, and fully transitioning over when confidence is high, otherwise reverting the release to the older version.
* More info about canary deployments at: https://martinfowler.com/bliki/CanaryRelease.html
* A blue/green deployment, is similar to the canary deployment where two deployments exist and when the new version is available and passes certain conditions, it can be ‘swapped’ for the new one, and otherwise reverting to the older version. Amazon has a guide for CodePipeline that can be used as a reference: https://aws.amazon.com/quickstart/architecture/blue-green-deployment/
