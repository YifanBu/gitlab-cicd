# Use Gitlab CI to build and deploy a Java App to AWS Elastic Beanstalk
1. Advanced CI Pipeline with code checks, unit tests, API tests, Performance tests and security checks
2. Publish test results both in HTML and XML format
3. Deploy to AWS Elastic Beanstalk

### Pipeline
Code -> Build -> Code Quality -> Tests -> Package -> Test -> Staging -> Production

### Artefact

The build artefact: `cars-api/build/libs/cars-api.jar`


### Images 
- openjdk:12-alpine
- amazon/aws-cli

### Variables
1. ARTIFACT_NAME
2. APP_NAME

### Gitlab Group
organize projects in a Gitlab group

group Settings -> CI/CD -> Variables -> `S3_BUCKET`, `AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY`