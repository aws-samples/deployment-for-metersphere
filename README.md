# Continuous Testing Platform based on MeterSphere

The solution is for deploying a continuous testing platform solution on AWS.
##  Target Audience
Who needs 
- A One-Click solution for setup a continuous testing platform on Amazon EC2
- A continuous testing platform with a visual user interface
- A Less Operation Effort solution via Amazon RDS

## Technical Details

### The Deployed Resources

The following resources were deployed using CloudFormation:

- Amazon EC2: deploys the main MeterSphere platform program using Docker. During test tasks, JMeter containers are started through Node Controller to perform the testing, and various result data is calculated and stored in the hosted database.
- Amazon Relational Database Service (Amazon RDS): used to store persistent data for the MeterSphere platform, such as test task data, interface configuration data, analysis result data, platform configuration, user information, and other data.