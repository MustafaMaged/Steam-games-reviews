# Steam-games-reviews
Process games reviews on steam with EMR cluster, and load it to amazon s3

## How to run:
This is the cluster I used for this project
```
aws emr create-cluster \
--name mussa_cluster \
--use-default-roles \
--release-label emr-5.28.0 \
--instance-count 4 \
--applications Name=Spark  \
--ec2-attributes KeyName=mussa-key,SubnetId=subnet-043b2242374dae257 \
--instance-type m5.xlarge \
--profile mustafa
```
