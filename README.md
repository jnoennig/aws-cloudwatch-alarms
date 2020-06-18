# CIS AWS Foundations Benchmarks CloudWatch Alarms

The CloudFormation template deploys CloudWatch filters and alarms for most of the CIS AWS Foundations Benchmarks.

## Prerequisites 

* CloudTrail trail enabled in all regions.
* CloudTrail trail read/write all events
* Ensure CloudTrail trail is integrated with CloudWatch Logs

## Deployment

The template only needs to be deployed in one region.

## Limitations

The emails you will receive from SNS will specify the region the alarm is located not the region the resource is located.

### Example

If the alarm is deployed in us-west-2 (Oregon) but you create a VPC in us-east-1 (N. Virginia) the email will only mention us-west-2.