# node.js
# node.js app deployment using AWS Beanstalk

# IAM : Elastic Beanstalk - Environments - Nodejs-beanstalk-env - Configuration - Configure service access - service role (this needs to have a new IAM service role for Beanstalk) for e.g. I have created service role - aws-elasticbeanstalk-service-role

# EC2 key pair - select one from already created list
# EC2 instance profile - select one from already created list

# CloudFormation - Stacks - Stack Info: 
# CloudFormation - Stacks - Events:
# will give give informations about the provisiong of AWS Beanstalk in this case

# Configure updates, monitoring, and logging - for CloudWatch Custom Metrics - Instance - select "Enhanced" - select few options for "Cloudwatch Metrics for Instance" and "Environment"

# Further down, Under rolling updates & deployments, select deployment policy as "immutable"

# to ssh the EC2 running Beanstalk
ssh -i "sam_key_pair.pem" root@ec2-3-225-115-141.compute-1.amazonaws.com 
# replace root with ec2-user
ssh -i "sam_key_pair.pem" ec2-user@ec2-3-225-115-141.compute-1.amazonaws.com


