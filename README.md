
### Design decision: 

#### for a minimal deploy use

- ec2 plus ebs (not scalable beyond a single machine)
- ec2 plus efs
- lambda plus efs

#### To do a longer function:
- Fire a SQS/SNS message to trigger another lambda and write back the data to storage